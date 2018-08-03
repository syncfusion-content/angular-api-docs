---
layout: post
title: Properties, Methods and Events of ejAccordion Widget
description: API reference for ejAccordion
documentation: API
platform: angular-api
keywords: accordion, ejAccordion, syncfusion, accordion api

---

# ejAccordion

The Accordion control is an interface where lists of items can be collapsed or expanded. It has several collapsible panels where only one can be expanded at a time that is useful for dashboards where space is limited. Each Accordion control has a template for its header and its content.



#### Example

{% highlight html %}

<ej-accordion>
    <h3>
        <a href="#">Twitter</a>
    </h3>
    <div>
        Twitter is an online social networking service that enables users to send and read short 140-character messages called "tweets".
        Registered users can read and post tweets, but those who are unregistered can only read them. Users access Twitter through the website interface, SMS or mobile device app Twitter Inc. is based in San Francisco and has more than 25 offices around the world.
        Twitter was created in March 2006 by Jack Dorsey, Evan Williams, Biz Stone, and Noah Glass and launched in July 2006. The service rapidly gained worldwide popularity, with more than 100 million users posting 340 million tweets a day in 2012.The service also handled 1.6 billion search queries per day.
    </div>
    <h3>
        <a href="#">Facebook</a>
    </h3>
    <div>
        Facebook is an online social networking service headquartered in Menlo Park, California. Its website was launched on February 4, 2004, by Mark Zuckerberg with his Harvard College roommates and fellow students Eduardo Saverin, Andrew McCollum, Dustin Moskovitz and Chris Hughes.The founders had initially limited the website's membership to Harvard students, but later expanded it to colleges in the Boston area, the Ivy League, and Stanford University. It gradually added support for students at various other universities and later to high-school students.
    </div>
    <h3>
        <a href="#">WhatsApp</a>
    </h3>
    <div>
        WhatsApp Messenger is a proprietary cross-platform instant messaging client for smart phones that operates under a subscription business model. It uses the Internet to send text messages, images, video, user location and audio media messages to other users using standard cellular mobile numbers.
        As of February 2016, WhatsApp had a user base of up to one billion,[10] making it the most globally popular messaging application.
        WhatsApp Inc., based in Mountain View, California, was acquired by Facebook Inc. on February 19, 2014, for approximately US$19.3 billion.
    </div>
</ej-accordion>

{% endhighlight %}

#### Requires

* module:jQuery

* module:jquery.easing.1.3.min.js

* module:ej.core.js

* module:ej.accordion.js


## Members

### ajaxSettings  `object`
{:#members:ajaxsettings}

Specifies the ajaxSettings option to load the content to the accordion control.

#### Default Value

* null

#### Example

{% highlight html %}

<ej-accordion ajaxSettings.type="GET" [ajaxSettings.cache]=false ajaxSettings.data={} ajaxSettings.dataType="html" ajaxSettings.contentType="html" [ajaxSettings.async]=true>
    <h3>
        <a href="#">Twitter</a>
    </h3>
    <div>
        Twitter is an online social networking service that enables users to send and read short 140-character messages called "tweets".
        Registered users can read and post tweets, but those who are unregistered can only read them. Users access Twitter through the website interface, SMS or mobile device app Twitter Inc. is based in San Francisco and has more than 25 offices around the world.
        Twitter was created in March 2006 by Jack Dorsey, Evan Williams, Biz Stone, and Noah Glass and launched in July 2006. The service rapidly gained worldwide popularity, with more than 100 million users posting 340 million tweets a day in 2012.The service also handled 1.6 billion search queries per day.
    </div>
    <h3>
        <a href="#">Facebook</a>
    </h3>
    <div>
        Facebook is an online social networking service headquartered in Menlo Park, California. Its website was launched on February 4, 2004, by Mark Zuckerberg with his Harvard College roommates and fellow students Eduardo Saverin, Andrew McCollum, Dustin Moskovitz and Chris Hughes.The founders had initially limited the website's membership to Harvard students, but later expanded it to colleges in the Boston area, the Ivy League, and Stanford University. It gradually added support for students at various other universities and later to high-school students.
    </div>
    <h3>
        <a href="#">WhatsApp</a>
    </h3>
    <div>
        WhatsApp Messenger is a proprietary cross-platform instant messaging client for smart phones that operates under a subscription business model. It uses the Internet to send text messages, images, video, user location and audio media messages to other users using standard cellular mobile numbers.
        As of February 2016, WhatsApp had a user base of up to one billion,[10] making it the most globally popular messaging application.
        WhatsApp Inc., based in Mountain View, California, was acquired by Facebook Inc. on February 19, 2014, for approximately US$19.3 billion.
    </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent { }

{% endhighlight %}


### ajaxSettings.async `boolean`
{:#members:ajaxsettings-async}

It specifies, whether to enable or disable asynchronous request.

### ajaxSettings.cache `boolean`
{:#members:ajaxsettings-cache}

It specifies the page will be cached in the web browser.

### ajaxSettings.contentType `string`
{:#members:ajaxsettings-contenttype}

It specifies the type of data is send in the query string.

### ajaxSettings.data `Object`
{:#members:ajaxsettings-data}

It specifies the data as an object, will be passed in the query string.

### ajaxSettings.dataType `string`
{:#members:ajaxsettings-datatype}

It specifies the type of data that you're expecting back from the response.

### ajaxSettings.type `string`
{:#members:ajaxsettings-type}

It specifies the HTTP request type.

### allowKeyboardNavigation `boolean`
{:#members:allowkeyboardnavigation}

Accordion headers can be expanded and collapsed on keyboard action.

#### Default Value

* true

#### Example

{% highlight html %}

<ej-accordion id="accordion" [allowKeyboardNavigation]=true>
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent { }

{% endhighlight %}


### collapseSpeed `number`
{:#members:collapsespeed}

To set the Accordion headers Collapse Speed.

#### Default Value

* 300

#### Example

{% highlight html %}

<ej-accordion id="accordion" collapseSpeed=500>
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent { }

{% endhighlight %}


### collapsible `boolean`
{:#members:collapsible}

Specifies the collapsible state of accordion control.

#### Default Value

* false

#### Example

{% highlight html %}

<ej-accordion id="accordion" [collapsible]=true>
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent { }

{% endhighlight %}

### cssClass `string`
{:#members:cssclass}

Sets the root CSS class for Accordion theme, which is used customize. 

#### Default Value

* ""

#### Example

{% highlight html %}

<ej-accordion id="accordion" [cssClass]="custom">
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent { }

{% endhighlight %}

{% highlight html %}

<style class="cssStyles">
    .custom {
        font-style: italic;
        text-align: justify;
    }
    .custom span.e-icon {
        display: none !important;
    }
    .custom h3 {
        text-decoration: underline;
        text-align: center;
    }
</style>

{% endhighlight %}



### customIcon `object`
{:#members:customicon}

Allows you to set the custom header Icon. It accepts two key values “header”, ”selectedHeader”.

1. header - The collapsing header CSS class name. 
2. selectedHeader - The active header CSS class name.


#### Default Value

* "{ header: "e-collapse", selectedHeader: "e-expand" }"

### customIcon.header `string`
{:#members:customicon-header}

This class name set to collapsing header. 

### customIcon.selectedHeader `string`
{:#members:customicon-selectedheader}

This class name set to expanded (active) header. 

#### Example

{% highlight html %}

<ej-accordion id="accordion" customIcon.header="header-close" customIcon.selectedHeader="header-expand">
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent { }

{% endhighlight %}

### disabledItems `number[]`
{:#members:disableditems}

Disables the specified indexed items in accordion.

N> The disabledItems is a dependent property of enableMultipleOpen. The enableMultipleOpen property should be set as true.


#### Default Value

* []

#### Example

{% highlight html %}

<ej-accordion id="accordion" [disabledItems]=" disabledItems">
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent { 
    disabledItems: array;
    constructor() {

 this.disabledItems=[0,1];
    }
}

{% endhighlight %}


### enableAnimation `boolean`
{:#members:enableanimation}

Specifies the animation behavior in accordion.

#### Default Value:

* true

#### Example

{% highlight html %}

<ej-accordion id="accordion" [enableAnimation]=false>
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent { }

{% endhighlight %}



### enabled `boolean`
{:#members:enabled}

With this enabled property, you can enable or disable the Accordion.

#### Default Value

* true

#### Example

{% highlight html %}

<ej-accordion id="accordion" [enabled]=true>
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent { }

{% endhighlight %}


### enabledItems `number[]`
{:#members:enableditems}

Used to enable the disabled items in accordion.

N> The enabledItems is a dependent property of enableMultipleOpen. The enableMultipleOpen property should be set as true.


#### Default Value

* []

#### Example

{% highlight html %}

<ej-accordion id="accordion" [enabledItems]="enabledItems">
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent { 
    enabledItems: array;
    constructor() {
    this.enabledItems=[0,1];
    }
}

{% endhighlight %}


### enableMultipleOpen `boolean`
{:#members:enablemultipleopen}

Multiple content panels to activate at a time.

#### Default Value

* false

#### Example

{% highlight html %}

<ej-accordion id="accordion" [enableMultipleOpen]=true>
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent { }

{% endhighlight %}


### enablePersistence `boolean`
{:#members:enablepersistence}

Save current model value to browser cookies for maintaining states. When refreshing the accordion control page, the model value is applied from browser cookies or HTML 5
local storage.

#### Default Value

* false

#### Example

{% highlight html %}

<ej-accordion id="accordion" [enablePersistence]=true>
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent { }

{% endhighlight %}


### enableRTL `boolean`
{:#members:enablertl}

Display headers and panel text from right-to-left.

#### Default Value

* false

#### Example

{% highlight html %}

<ej-accordion id="accordion" [enableRTL]=true>
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent { }

{% endhighlight %}


### events `string`
{:#members:events}

The events API binds the action for activating the accordion header. Users can activate the header by using mouse actions such as mouse-over, mouse-up, mouse-down, and so
on.

#### Default Value

* "click"

#### Example

{% highlight html %}

<ej-accordion id="accordion" events="mouseover">
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent { }

{% endhighlight %}


### expandSpeed `number`
{:#members:expandspeed}

To set the Accordion headers Expand Speed.

#### Default Value:

* 300

#### Example

{% highlight html %}

<ej-accordion id="accordion" expandSpeed=500>
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent { }

{% endhighlight %}



### headerSize `number|string`
{:#members:headersize}

Sets the height for Accordion items header.

#### Example

{% highlight html %}

<ej-accordion id="accordion" headerSize="40px">
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent { }

{% endhighlight %}


### height `number|string`
{:#members:height}

Specifies height of the accordion.

#### Default Value:

* null

#### Example

{% highlight html %}

<ej-accordion id="accordion" height="500px">
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent { }

{% endhighlight %}


### heightAdjustMode `enum|string`
{:#members:heightadjustmode}

<ts name="ej.Accordion.HeightAdjustMode" />

Adjusts the content panel height based on the given option (content, auto, or fill). By default, the panel heights are adjusted based on the content. 


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
Content</td>
<td class="description">Height fit to the content in the panel</td>
</tr>
<tr>
<td class="name">
Auto</td>
<td class="description">Height set to the largest content in the panel</td>
</tr>
<tr>
<td class="name">
Fill</td>
<td class="description">Height filled to the content of the panel</td>
</tr>
</tbody>
</table>


#### Default Value

* "content"

#### Example

{% highlight html %}

<ej-accordion id="accordion" [heightAdjustMode]="mode">
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
    mode:any;

//heightAdjustMode  for content div on initialization. 
    constructor() { 
    this.mode=ej.Accordion.HeightAdjustMode.Auto;//enum
    }
}

{% endhighlight %}

{% highlight html %}

<ej-accordion id="accordion" [heightAdjustMode]="mode">
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
    mode:any;


    constructor() { 
    //Pass value on string type. 
    this.mode="auto";
    }
}

{% endhighlight %}





### htmlAttributes `object`
{:#members:htmlattributes}

It allows to define the characteristics of the Accordion control. It will helps to extend the capability of an HTML element.

#### Default Value

* {}

#### Example

{% highlight html %}

<ej-accordion id="accordion" [htmlAttributes ]="htmlAttributes" [collapsible]=true>
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
    htmlAttributes : any;
    constructor() { 
    this.htmlAttributes = { title: "Demo" };
    }
}

{% endhighlight %}


### selectedItemIndex `number`
{:#members:selecteditemindex}

The given index header will activate (open). If collapsible is set to true, and a negative value is given, then all headers are collapsed. Otherwise, the first panel is
activated.

#### Default Value

* 0

#### Example

{% highlight html %}

<ej-accordion id="accordion" selectedItemIndex=1>
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent { }

{% endhighlight %}

### selectedItems `number[]`
{:#members:selecteditems}

Activate the specified indexed items of the accordion

N> The selectedItems is a dependent property of enableMultipleOpen. The enableMultipleOpen property should be set as true.


#### Default Value

* [0]

#### Example

{% highlight html %}

<ej-accordion id="accordion" [enableMultipleOpen]=true [selectedItems]="selectedItems">
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent { 
    selectedItems: array;
    constructor() {

 this.selectedItems=[0,1];
    }
}

{% endhighlight %}


### showCloseButton `boolean`
{:#members:showclosebutton}

Used to determines the close button visibility an each accordion items. This close button helps to remove the accordion item from the control.  

#### Default Value

* false

#### Example

{% highlight html %}

<ej-accordion id="accordion" [showCloseButton]=true>
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent { }

{% endhighlight %}


### showRoundedCorner `boolean`
{:#members:showroundedcorner}

Displays rounded corner borders on the Accordion control's panels and headers.

#### Default Value

* false

#### Example

{% highlight html %}

<ej-accordion id="accordion" [showRoundedCorner]=true>
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent { }

{% endhighlight %}

### width `number|string`
{:#members:width}

Specifies width of the accordion.

#### Default Value:

* null

#### Example

{% highlight html %}

<ej-accordion id="accordion" [collapsible]=true>
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent { }

{% endhighlight %}


## Methods

### addItem(header_name, content, index, isAjaxReq)
{:#methods:additem}

AddItem method is used to add the panel in dynamically. It receives the following parameters


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
header_name</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">specify the name of the header</td>
</tr>
<tr>
<td class="name">
content</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">content of the new panel</td>
</tr>
<tr>
<td class="name">
index</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">insertion place of the new panel</td>
</tr>
<tr>
<td class="name">
isAjaxReq</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Enable or disable the AJAX request to the added panel</td>
</tr>
</tbody>
</table>



#### Example

{% highlight html %}

<ej-accordion id="accordion" (create)="create()">
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {    
    constructor() {
    }
create() {

  var Object = $("#accordion").data("ejAccordion");
      Object.addItem("New item", "The accordion content", 2);

}
}

{% endhighlight %}

{% highlight html %}

<ej-accordion id="accordion" (create)="create()">
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {    
    constructor() {
    }
create() {

  $("#accordion").ejAccordion("addItem", "New Item", "The accordion content", 2);

}
}

{% endhighlight %}




### collapseAll()
{:#methods:collapseall}

This method used to collapse the all the expanded items in accordion at a time.

N>  Before we call this method, we must set "collapsible" is true. Then only collapseAll method will working.


#### Example

{% highlight html %}

<ej-accordion id="accordion" [collapsible]=true (create)="create()">
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {    
    constructor() {
    }
create() {

  var Object = $("#accordion").data("ejAccordion");
      Object.collapseAll();

}
}

{% endhighlight %}

{% highlight html %}

<ej-accordion id="accordion" [collapsible]=true (create)="create()">
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {    
    constructor() {
    }
create() {

  $("#accordion").ejAccordion("collapseAll");

}
}

{% endhighlight %}





### collapsePanel()
{:#methods:collapsepanel}

This method used to Collapses the specified items in accordion at a time.


#### Example

{% highlight html %}

<ej-accordion id="accordion" [collapsible]=true (create)="create()">
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {    
    constructor() {
    }
create() {

  var Object = $("#accordion").data("ejAccordion");
      Object.collapsePanel(0);

}
}

{% endhighlight %}

{% highlight html %}

<ej-accordion id="accordion" [collapsible]=true (create)="create()">
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {    
    constructor() {
    }
create() {

  $("#accordion").ejAccordion("collapsePanel",0);

}
}

{% endhighlight %}





### destroy()
{:#methods:destroy}

destroy the Accordion widget all events bound using this._on will be unbind automatically and bring the control to pre-init state.

#### Example

{% highlight html %}

<ej-accordion id="accordion">
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

<button type="button" (click)="onClick()">DESTROY</button>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {    
    constructor() {
    }
onClick() {

  var Object = $("#accordion").data("ejAccordion");
      Object.destroy();

}
}

{% endhighlight %}

{% highlight html %}

<ej-accordion id="accordion">
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

<button type="button" (click)="onClick()">DESTROY</button>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {    
    constructor() {
    }
onClick() {

  $("#accordion").ejAccordion("destroy");

}
}

{% endhighlight %}





### disable()
{:#methods:disable}

Disables the accordion widget includes all the headers and content panels.

#### Example

{% highlight html %}

<ej-accordion id="accordion" [collapsible]=true (create)="create()">
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {    
    constructor() {
    }
create() {

  var Object = $("#accordion").data("ejAccordion");
      Object.disable();

}
}

{% endhighlight %}

{% highlight html %}

<ej-accordion id="accordion" [collapsible]=true (create)="create()">
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {    
    constructor() {
    }
create() {

  $("#accordion").ejAccordion("disable");

}
}

{% endhighlight %}






### disableItems(index)
{:#methods:disableitems}

Disable the accordion widget item based on specified header index.


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
index</td>
<td class="type"><span class="param-type">array</span></td>
<td class="description">index values to disable the panels</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<ej-accordion id="accordion" (create)="create()">
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {    
    constructor() {
    }
create() {

  var Object = $("#accordion").data("ejAccordion");
      Object.disableItems([1]);

}
}

{% endhighlight %}

{% highlight html %}

<ej-accordion id="accordion" (create)="create()">
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {    
    constructor() {
    }
create() {

  $("#accordion").ejAccordion("disableItems", [1]);

}
}

{% endhighlight %}




### enable()
{:#methods:enable}


Enable the accordion widget includes all the headers and content panels.


#### Example

{% highlight html %}

<ej-accordion id="accordion" [collapsible]=true (create)="create()">
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {    
    constructor() {
    }
create() {

  var Object = $("#accordion").data("ejAccordion");
      Object.enable();

}
}

{% endhighlight %}

{% highlight html %}

<ej-accordion id="accordion" [collapsible]=true (create)="create()">
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {    
    constructor() {
    }
create() {

  $("#accordion").ejAccordion("enable");

}
}

{% endhighlight %}








### enableItems(index)
{:#methods:enableitems}

Enable the accordion widget item based on specified header index.


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
index</td>
<td class="type"><span class="param-type">array</span></td>
<td class="description">index values to enable the panels</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<ej-accordion id="accordion" (create)="create()">
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {    
    constructor() {
    }
create() {

  var Object = $("#accordion").data("ejAccordion");
      Object.disableItems([0]);
      Object.disableItems([1]);
      Object.enableItems([1]);

}
}

{% endhighlight %}

{% highlight html %}

<ej-accordion id="accordion" (create)="create()">
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {    
    constructor() {
    }
create() {
      $("#accordion").ejAccordion("disableItems", [0]); 

  $("#accordion").ejAccordion("disableItems", [1]); 

  $("#accordion").ejAccordion("enableItems", [1]);

}
}

{% endhighlight %}







### expandAll()
{:#methods:expandall}

To expand all the accordion widget items.

N>  Before we call this method, we must set "enableMultipleOpen" is true. Then only expandAll method will working.


#### Example

{% highlight html %}

<ej-accordion id="accordion" [enableMultipleOpen]=true (create)="create()">
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {    
    constructor() {
    }
create() {

  var Object = $("#accordion").data("ejAccordion");
      Object.expandAll();

}
}

{% endhighlight %}

{% highlight html %}

<ej-accordion id="accordion" [enableMultipleOpen]=true (create)="create()">
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {    
    constructor() {
    }
create() {

  $("#accordion").ejAccordion("expandAll");

}
}

{% endhighlight %}






### expandPanel()
{:#methods:expandpanel}

This method used to Expand the specified items in accordion at a time.

#### Example

{% highlight html %}

<ej-accordion id="accordion" (create)="create()">
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {    
    constructor() {
    }
create() {

  var Object = $("#accordion").data("ejAccordion");
      Object.expandPanel(1);

}
}

{% endhighlight %}

{% highlight html %}

<ej-accordion id="accordion" (create)="create()">
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {    
    constructor() {
    }
create() {

  $("#accordion").ejAccordion("expandPanel",1);

}
}

{% endhighlight %}







### getItemsCount()
{:#methods:getitemscount}

Returns the total number of panels in the control.


#### Returns:
{:#methods:returns:}

number


#### Example

{% highlight html %}

<ej-accordion id="accordion" (create)="create()">
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {    
    constructor() {
    }
create() {

  var Object = $("#accordion").data("ejAccordion");
      Object.getItemsCount();

}
}

{% endhighlight %}

{% highlight html %}

<ej-accordion id="accordion" (create)="create()">
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {    
    constructor() {
    }
create() {

  $("#accordion").ejAccordion("getItemsCount");

}
}

{% endhighlight %}








### hide()
{:#methods:hide}

Hides the visible Accordion control.

#### Example

{% highlight html %}

<ej-accordion id="accordion" (create)="create()">
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {    
    constructor() {
    }
create() {

  var Object = $("#accordion").data("ejAccordion");
      Object.hide();

}
}

{% endhighlight %}

{% highlight html %}

<ej-accordion id="accordion" (create)="create()">
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {    
    constructor() {
    }
create() {

  $("#accordion").ejAccordion("hide");

}
}

{% endhighlight %}





### refresh()
{:#methods:refresh}

The refresh method is used to adjust the control size based on the parent element dimension.

#### Example

{% highlight html %}

<ej-accordion id="accordion" (create)="create()">
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {    
    constructor() {
    }
create() {

  var Object = $("#accordion").data("ejAccordion");
      Object.refresh();

}
}

{% endhighlight %}

{% highlight html %}

<ej-accordion id="accordion" (create)="create()">
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {    
    constructor() {
    }
create() {

  $("#accordion").ejAccordion("refresh");

}
}

{% endhighlight %}







### removeItem(index)
{:#methods:removeitem}

RemoveItem method is used to remove the specified index panel.It receives the parameter as number.
  

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
index </td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">specify the index value for remove the accordion panel.</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<ej-accordion id="accordion" (create)="create()">
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {    
    constructor() {
    }
create() {

  var Object = $("#accordion").data("ejAccordion");
      Object.removeItem(2);

}
}

{% endhighlight %}

{% highlight html %}

<ej-accordion id="accordion" (create)="create()">
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {    
    constructor() {
    }
create() {

  $("#accordion").ejAccordion("removeItem", 2);

}
}

{% endhighlight %}







### show()
{:#methods:show}


Shows the hidden Accordion control.


#### Example

{% highlight html %}

<ej-accordion id="accordion" (create)="create()">
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {    
    constructor() {
    }
create() {

  var Object = $("#accordion").data("ejAccordion");
      Object.show();

}
}

{% endhighlight %}

{% highlight html %}

<ej-accordion id="accordion" (create)="create()">
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {    
    constructor() {
    }
create() {

  $("#accordion").ejAccordion("show");

}
}

{% endhighlight %}








## Events

### activate
{:#events:activate}


Triggered after a Accordion item is active . Argument values are activeIndex, activeHeader, isInteraction and current model values.


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
 cancel </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
 model </td>
<td class="type"><ts ref="ej.Accordion.Model"/><span class="param-type">object</span></td>
<td class="description">returns the accordion model</td>
</tr>
<tr>
<td class="name">
 type </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
 activeIndex </td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns active index</td>
</tr>
<tr>
<td class="name">
 activeHeader </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns current active header</td>
</tr>
<tr>
<td class="name">
 isInteraction </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">returns true when the Accordion index activated by user interaction otherwise returns false</td>
</tr>
</tbody>
</table>



#### Example

{% highlight html %}

<ej-accordion id="accordion" (activate)="activate($event)">
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent { 
    activate(args) {
        //do the changes
    }
}

{% endhighlight %}





### ajaxBeforeLoad
{:#events:ajaxbeforeload}

Triggered before the AJAX content is loaded in a content panel. Arguments have location of the content (URL) and current model value.


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
 cancel </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
 model </td>
<td class="type"><ts ref="ej.Accordion.Model"/><span class="param-type">object</span></td>
<td class="description">returns the accordion model</td>
</tr>
<tr>
<td class="name">
 type </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
 URL </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns current AJAX content location</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<ej-accordion id="accordion" (ajaxBeforeLoad)=" ajaxBeforeLoad($event)" ajaxSettings.type="GET" [ajaxSettings.cache]=false ajaxSettings.data={} ajaxSettings.dataType="html" ajaxSettings.contentType="html" [ajaxSettings.async]=true>
   <h3>
           <a href="../aspnet.html">ASP.NET</a></h3>
       <div>
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent { 
     ajaxBeforeLoad(args) {
        //do the changes
    }
}

{% endhighlight %}





### ajaxError
{:#events:ajaxerror}


Triggered after AJAX load failed action. Arguments have URL, error message, and current model value.


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
 cancel </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
 model </td>
<td class="type"><ts ref="ej.Accordion.Model"/><span class="param-type">object</span></td>
<td class="description">returns the accordion model</td>
</tr>
<tr>
<td class="name">
 type </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
 URL </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns current AJAX content location</td>
</tr>
<tr>
<td class="name">
 data </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the failed data sent.</td>
</tr>
</tbody>
</table>



#### Example

{% highlight html %}

<ej-accordion id="accordion" (ajaxError)=" ajaxError($event)" ajaxSettings.type="GET" [ajaxSettings.cache]=false ajaxSettings.data={} ajaxSettings.dataType="html" ajaxSettings.contentType="html" [ajaxSettings.async]=true>
   <h3>
           <a href="../aspnet.html">ASP.NET</a></h3>
       <div>
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent { 
     ajaxError(args) {
        //do the changes
    }
}

{% endhighlight %}


### ajaxLoad
{:#events:ajaxload}


Triggered after the AJAX content loads. Arguments have current model values.


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
 cancel </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
 model </td>
<td class="type"><ts ref="ej.Accordion.Model"/><span class="param-type">object</span></td>
<td class="description">returns the accordion model</td>
</tr>
<tr>
<td class="name">
 type </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
 URL </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the URL</td>
</tr>
</tbody>
</table>



#### Example

{% highlight html %}

<ej-accordion id="accordion" (ajaxLoad)=" ajaxLoad($event)" ajaxSettings.type="GET" [ajaxSettings.cache]=false ajaxSettings.data={} ajaxSettings.dataType="html" ajaxSettings.contentType="html" [ajaxSettings.async]=true>
   <h3>
           <a href="../aspnet.html">ASP.NET</a></h3>
       <div>
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent { 
     ajaxLoad(args) {
        //do the changes
    }
}

{% endhighlight %}





### ajaxSuccess
{:#events:ajaxsuccess}


Triggered after AJAX success action. Arguments have URL, content, and current model values.


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
 cancel </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
 model </td>
<td class="type"><ts ref="ej.Accordion.Model"/><span class="param-type">object</span></td>
<td class="description">returns the accordion model</td>
</tr>
<tr>
<td class="name">
 type </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
 URL </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns current AJAX content location</td>
</tr>
<tr>
<td class="name">
 data </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the successful data sent.</td>
</tr>
<tr>
<td class="name">
 content </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the AJAX content.</td>
</tr>
</tbody>
</table>



#### Example

{% highlight html %}

<ej-accordion id="accordion" (ajaxSuccess)=" ajaxSuccess($event)" ajaxSettings.type="GET" [ajaxSettings.cache]=false ajaxSettings.data={} ajaxSettings.dataType="html" ajaxSettings.contentType="html" [ajaxSettings.async]=true>
   <h3>
           <a href="../aspnet.html">ASP.NET</a></h3>
       <div>
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent { 
     ajaxSuccess(args) {
        //do the changes
    }
}

{% endhighlight %}





### beforeActivate
{:#events:beforeactivate}




Triggered before a tab item is active. Arguments have active index and model values.

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
 cancel </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
 model </td>
<td class="type"><ts ref="ej.Accordion.Model"/><span class="param-type">object</span></td>
<td class="description">returns the accordion model</td>
</tr>
<tr>
<td class="name">
 type </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
 activeIndex </td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns active index</td>
</tr>
<tr>
<td class="name">
 isInteraction </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">returns true when the Accordion index activated by user interaction otherwise returns false</td>
</tr>
</tbody>
</table>



#### Example

{% highlight html %}

<ej-accordion id="accordion" (beforeActivate)="beforeActivate($event)">
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent { 
    beforeActivate(args) {
        //do the changes
    }
}

{% endhighlight %}



### beforeInactivate
{:#events:beforeinactivate}

Triggered before a Accordion item is inactive. Argument values are  inActiveIndex and  model values.

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
 cancel </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
 model </td>
<td class="type"><ts ref="ej.Accordion.Model"/><span class="param-type">object</span></td>
<td class="description">returns the accordion model</td>
</tr>
<tr>
<td class="name">
 type </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
 inActiveIndex </td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns active index</td>
</tr>
<tr>
<td class="name">
 isInteraction </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">returns true when the Accordion index activated by user interaction otherwise returns false</td>
</tr>
</tbody>
</table>



#### Example

{% highlight html %}

<ej-accordion id="accordion" (beforeInActivate)="beforeInActivate($event)">
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent { 
    beforeInActivate(args) {
        //do the changes
    }
}

{% endhighlight %}



### create
{:#events:create}

Triggered after Accordion control creation.

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
 cancel </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
 model </td>
<td class="type"><ts ref="ej.Accordion.Model"/><span class="param-type">object</span></td>
<td class="description">returns the accordion model</td>
</tr>
<tr>
<td class="name">
 type </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<ej-accordion id="accordion" (create)="create($event)">
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent { 
    create(args) {
        //do the changes
    }
}

{% endhighlight %}




### destroy
{:#events:destroy}

Triggered after Accordion control destroy.

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
 cancel </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
 model </td>
<td class="type"><ts ref="ej.Accordion.Model"/><span class="param-type">object</span></td>
<td class="description">returns the accordion model</td>
</tr>
<tr>
<td class="name">
 type </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
</tbody>
</table>



#### Example

{% highlight html %}

<ej-accordion id="accordion" (destroy)="destroy($event)">
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent { 
    destroy(args) {
        //do the changes
    }
}

{% endhighlight %}



### inActivate
{:#events:inactivate}

Triggered after a Accordion item is inactive. Argument values are  inActiveHeader, inActiveIndex ,isInteraction and current model values.


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
 cancel </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
 model </td>
<td class="type"><ts ref="ej.Accordion.Model"/><span class="param-type">object</span></td>
<td class="description">returns the accordion model</td>
</tr>
<tr>
<td class="name">
 type </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
 inActiveIndex </td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns active index</td>
</tr>
<tr>
<td class="name">
 inActiveHeader </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns in active element</td>
</tr>
<tr>
<td class="name">
 isInteraction </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">returns true when the Accordion index activated by user interaction otherwise returns false</td>
</tr>
</tbody>
</table>



#### Example

{% highlight html %}

<ej-accordion id="accordion" (inActivate)="inActivate($event)">
   <h3>
           <a href="#">ASP.NET</a></h3>
       <div>
Microsoft ASP.NET is a set of technologies in the Microsoft .NET Framework for building Web applications and XML Web services. ASP.NET pages execute on the server and generate markup such as HTML, WML, or XML that is sent to a desktop or mobile browser.
       </div>
       <h3>
           <a href="#">ASP.NET MVC</a></h3>
       <div>
The Model-View-Controller (MVC) architectural pattern separates an application into three main components: the model, the view, and the controller. The ASP.NET MVC framework provides an alternative to the ASP.NET Web Forms pattern for creating Web applications.
       </div>
       <h3>
           <a href="#">JavaScript</a></h3>
       <div>
JavaScript (JS) is an interpreted computer programming language. It was originally implemented as part of web browsers so that client-side scripts could interact with the user, control the browser, communicate asynchronously, and alter the document content that was displayed.
       </div>
</ej-accordion>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent { 
    inActivate(args) {
        //do the changes
    }
}

{% endhighlight %}



