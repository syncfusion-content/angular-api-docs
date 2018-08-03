---
layout: post
title: Properties, Methods and Events of ejTab Widget
description: API reference for ejTab
documentation: API
platform: angular-api
keywords: Tab, ejTab, syncfusion, Tab api 
---

# ejTab



The Tab control is an interface where list of items are expanded from a single item. Each Tab panel defines its header text or header template, as well as a content template. Tab items are dynamically added and removed. Tabs can be loaded with AJAX content that is useful for building dashboards where space is limited.











#### Example

{% highlight html %}

<ej-tab id="tab">
    <ul>
        <li><a href="#twitter">Twitter</a></li>
        <li><a href="#facebook">Facebook</a></li>
        <li><a href="#whatsapp">WhatsApp</a></li>
    </ul>
    <div id="twitter">
        Twitter is an online social networking service that enables users to send and read short 140-character messages called "tweets".
        Registered users can read and post tweets, but those who are unregistered can only read them. Users access Twitter through the website interface, SMS or mobile device app Twitter Inc. is based in San Francisco and has more than 25 offices around the world.
        Twitter was created in March 2006 by Jack Dorsey, Evan Williams, Biz Stone, and Noah Glass and launched in July 2006. The service rapidly gained worldwide popularity, with more than 100 million users posting 340 million tweets a day in 2012.The service also handled 1.6 billion search queries per day.
    </div>
    <div id="facebook">
        Facebook is an online social networking service headquartered in Menlo Park, California. Its website was launched on February 4, 2004, by Mark Zuckerberg with his Harvard College roommates and fellow students Eduardo Saverin, Andrew McCollum, Dustin Moskovitz and Chris Hughes.The founders had initially limited the website's membership to Harvard students, but later expanded it to colleges in the Boston area, the Ivy League, and Stanford University. It gradually added support for students at various other universities and later to high-school students.
    </div>
    <div id="whatsapp">
        WhatsApp Messenger is a proprietary cross-platform instant messaging client for smart phones that operates under a subscription business model. It uses the Internet to send text messages, images, video, user location and audio media messages to other users using standard cellular mobile numbers.
        As of February 2016, WhatsApp had a user base of up to one billion,[10] making it the most globally popular messaging application.
        WhatsApp Inc., based in Mountain View, California, was acquired by Facebook Inc. on February 19, 2014, for approximately US$19.3 billion.
    </div>
</ej-tab>

{% endhighlight %}




#### Requires



* module:jQuery

* module:jquery.easing.1.3.min.js

* module:ej.core.js

* module:ej.tab.js


## Members




### ajaxSettings `object`
{:#members:ajaxsettings}




Specifies the ajaxSettings option to load the content to the Tab control.




#### Example

{% highlight html %}


<div id="dish" style="width: 650px">
<ej-tab id="dishtype">
    <ul>
        <li><a href="#pizza">Pizza Menu</a></li>
        <li><a href="#sandwich">Sandwich Menu</a></li>
    </ul>
    <div id="pizza" style="background-color: #F5F5F5">
        <p>Pizza cooked to perfection tossed with milk, vegetables, potatoes, poultry, 100% pure mutton, and cheese - and in creating nutritious and tasty meals to maintain good health.</p>
        <div id="pizza">
        <ej-tab id="pizza" [ajaxSettings.dataType]="dataType" [ajaxSettings.contentType]="contentType" [ajaxSettings.async]="async" [ajaxSettings.data]="data" [ajaxSettings.type]="type" [ajaxSettings.cache]="cache">
            <ul>
                <li>
                    <a href="content/cornSpinach.html">Corn & Spinach </a></li>
                <li>
                    <a href="Content/chickenDelite.html">Chicken Delite </a></li>
            </ul>
        </ej-tab>
        </div>
    </div>
    <div id="sandwich" style="background-color: #F5F5F5">
        <p>Sandwich cooked to perfection tossed with bread, milk, vegetables, potatoes, poultry, 100% pure mutton, and cheese - and in creating nutritious and tasty meals to maintain good health.</p>
        <div id="sandwich">
        <ej-tab id="sandwich" [ajaxSettings.dataType]="dataType" [ajaxSettings.contentType]="contentType" [ajaxSettings.async]="async" [ajaxSettings.data]="data" [ajaxSettings.type]="type" [ajaxSettings.cache]="cache">
            <ul>
                <li>
                    <a href="Content/gardenVeggie.html">Garden Veggie </a></li>
                <li>
                    <a href="Content/chickenTikka.html">Chicken Tikka </a></li>
                <li>
                    <a href="Content/paneerTikka.html">Paneer Tikka </a></li>
            </ul>
            </ej-tab>
        </div>
    </div>
    </ej-tab>
</div>


{% endhighlight %}


{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './tab.component.html',
    styleUrls: ['./tab.component.css'],
    encapsulation: ViewEncapsulation.None,
})
export class ScrollTabComponent {
    dataType: any;

contentType: any;

async: any;
    cache: any;
    data: Object;
    type: any;
    constructor() {
        this.cache= false;
        this.data= {};
        this.type= 'GET';
    
this.dataType= "html";


this.contentType= "html";


this.async= true;
    }
} 

{% endhighlight %}

The file ‘**cornSpinach.html**’ content is as follows. 

{% highlight html %}


    <div class="e-content">
        <img src="http://js.syncfusion.com/demos/web/images/accordion/corn-and-spinach-05.png" alt="corn-spinach"/>
        <div class="ingredients">
            Rate    : $70<br />
            Ingredients : cheese, sweet corn &amp; green capsicums.
                <br />
            Description: Small pizza bases are topped with spinach and Paneer and fresh cream, a nice layer of mozzarella cheese. This is baked until the cheese is all hot and gooey.                   
        </div>
    </div>


{% endhighlight %}



The file ‘**chickenDelite.html’** content is as follows.

{% highlight html %}


    <div class="e-content">
        <img src="http://js.syncfusion.com/demos/web/images/accordion/chicken-delite.png" alt="chicken-delite"/>
        <div class="ingredients">
            Rate    : $100<br />
            Ingredients : cheese, chicken chunks, onions &amp; pineapple chunks.  
            <br />
            Description: This is a tasty, elegant chicken dish that is easy to prepare.
        </div>
    </div>


{% endhighlight %}






### ajaxSettings.async `boolean`
{:#members:ajaxsettings-async}




It specifies, whether to enable or disable asynchronous request.


#### Default Value




* true



### ajaxSettings.cache `boolean`
{:#members:ajaxsettings-cache}




It specifies the page will be cached in the web browser.




#### Default Value




* false




### ajaxSettings.contentType `string`
{:#members:ajaxsettings-contenttype}




It specifies the type of data is send in the query string.



#### Default Value




* "html"



### ajaxSettings.data `object`
{:#members:ajaxsettings-data}




It specifies the data as an object, will be passed in the query string.



#### Default Value




* {}



### ajaxSettings.dataType `string`
{:#members:ajaxsettings-datatype}




It specifies the type of data that you're expecting back from the response.



#### Default Value




* "html"


### ajaxSettings.type `string`
{:#members:ajaxsettings-type}




It specifies the HTTP request type.



#### Default Value




* "get"


### allowKeyboardNavigation `boolean`
{:#members:allowkeyboardnavigation}




Tab items interaction with keyboard keys, like headers active navigation.


#### Default Value




* true




#### Example

{% highlight html %}

<ej-tab id="tab" [allowKeyboardNavigation]=true>
    <ul>
        <li><a href="#twitter">Twitter</a></li>
        <li><a href="#facebook">Facebook</a></li>
        <li><a href="#whatsapp">WhatsApp</a></li>
    </ul>
    <div id="twitter">
        Twitter is an online social networking service that enables users to send and read short 140-character messages called "tweets".
        Registered users can read and post tweets, but those who are unregistered can only read them. Users access Twitter through the website interface, SMS or mobile device app Twitter Inc. is based in San Francisco and has more than 25 offices around the world.
        Twitter was created in March 2006 by Jack Dorsey, Evan Williams, Biz Stone, and Noah Glass and launched in July 2006. The service rapidly gained worldwide popularity, with more than 100 million users posting 340 million tweets a day in 2012.The service also handled 1.6 billion search queries per day.
    </div>
    <div id="facebook">
        Facebook is an online social networking service headquartered in Menlo Park, California. Its website was launched on February 4, 2004, by Mark Zuckerberg with his Harvard College roommates and fellow students Eduardo Saverin, Andrew McCollum, Dustin Moskovitz and Chris Hughes.The founders had initially limited the website's membership to Harvard students, but later expanded it to colleges in the Boston area, the Ivy League, and Stanford University. It gradually added support for students at various other universities and later to high-school students.
    </div>
    <div id="whatsapp">
        WhatsApp Messenger is a proprietary cross-platform instant messaging client for smart phones that operates under a subscription business model. It uses the Internet to send text messages, images, video, user location and audio media messages to other users using standard cellular mobile numbers.
        As of February 2016, WhatsApp had a user base of up to one billion,[10] making it the most globally popular messaging application.
        WhatsApp Inc., based in Mountain View, California, was acquired by Facebook Inc. on February 19, 2014, for approximately US$19.3 billion.
    </div>
</ej-tab>

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
}


{% endhighlight %}




### collapsible `boolean`
{:#members:collapsible}




Allow to collapsing the active item, while click on the active header.


#### Default Value




* false




#### Example

{% highlight html %}

<ej-tab id="tab" [collapsible]=true>
    <ul>
        <li><a href="#twitter">Twitter</a></li>
        <li><a href="#facebook">Facebook</a></li>
        <li><a href="#whatsapp">WhatsApp</a></li>
    </ul>
    <div id="twitter">
        Twitter is an online social networking service that enables users to send and read short 140-character messages called "tweets".
        Registered users can read and post tweets, but those who are unregistered can only read them. Users access Twitter through the website interface, SMS or mobile device app Twitter Inc. is based in San Francisco and has more than 25 offices around the world.
        Twitter was created in March 2006 by Jack Dorsey, Evan Williams, Biz Stone, and Noah Glass and launched in July 2006. The service rapidly gained worldwide popularity, with more than 100 million users posting 340 million tweets a day in 2012.The service also handled 1.6 billion search queries per day.
    </div>
    <div id="facebook">
        Facebook is an online social networking service headquartered in Menlo Park, California. Its website was launched on February 4, 2004, by Mark Zuckerberg with his Harvard College roommates and fellow students Eduardo Saverin, Andrew McCollum, Dustin Moskovitz and Chris Hughes.The founders had initially limited the website's membership to Harvard students, but later expanded it to colleges in the Boston area, the Ivy League, and Stanford University. It gradually added support for students at various other universities and later to high-school students.
    </div>
    <div id="whatsapp">
        WhatsApp Messenger is a proprietary cross-platform instant messaging client for smart phones that operates under a subscription business model. It uses the Internet to send text messages, images, video, user location and audio media messages to other users using standard cellular mobile numbers.
        As of February 2016, WhatsApp had a user base of up to one billion,[10] making it the most globally popular messaging application.
        WhatsApp Inc., based in Mountain View, California, was acquired by Facebook Inc. on February 19, 2014, for approximately US$19.3 billion.
    </div>
</ej-tab>

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
}


{% endhighlight %}




### cssClass `string`
{:#members:cssclass}




Set the root class for Tab theme. This cssClass API helps to use custom skinning option for Tab control.


#### Default Value




* ""




#### Example

{% highlight html %}

<ej-tab id="tab" cssClass="cssClass">
    <ul>
        <li><a href="#twitter">Twitter</a></li>
        <li><a href="#facebook">Facebook</a></li>
        <li><a href="#whatsapp">WhatsApp</a></li>
    </ul>
    <div id="twitter">
        Twitter is an online social networking service that enables users to send and read short 140-character messages called "tweets".
        Registered users can read and post tweets, but those who are unregistered can only read them. Users access Twitter through the website interface, SMS or mobile device app Twitter Inc. is based in San Francisco and has more than 25 offices around the world.
        Twitter was created in March 2006 by Jack Dorsey, Evan Williams, Biz Stone, and Noah Glass and launched in July 2006. The service rapidly gained worldwide popularity, with more than 100 million users posting 340 million tweets a day in 2012.The service also handled 1.6 billion search queries per day.
    </div>
    <div id="facebook">
        Facebook is an online social networking service headquartered in Menlo Park, California. Its website was launched on February 4, 2004, by Mark Zuckerberg with his Harvard College roommates and fellow students Eduardo Saverin, Andrew McCollum, Dustin Moskovitz and Chris Hughes.The founders had initially limited the website's membership to Harvard students, but later expanded it to colleges in the Boston area, the Ivy League, and Stanford University. It gradually added support for students at various other universities and later to high-school students.
    </div>
    <div id="whatsapp">
        WhatsApp Messenger is a proprietary cross-platform instant messaging client for smart phones that operates under a subscription business model. It uses the Internet to send text messages, images, video, user location and audio media messages to other users using standard cellular mobile numbers.
        As of February 2016, WhatsApp had a user base of up to one billion,[10] making it the most globally popular messaging application.
        WhatsApp Inc., based in Mountain View, California, was acquired by Facebook Inc. on February 19, 2014, for approximately US$19.3 billion.
    </div>
</ej-tab>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import {ViewEncapsulation} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html',
    styleUrls: ['./tab.component.css'],
    encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent {
    
    constructor() {
       
    }
}

{% endhighlight %}

The css must be defined in stylesheet.

{% highlight ts %}

<style>
.cssClass{
    font-size: 20px;
}
</style>

{% endhighlight %}




### disabledItemIndex `number[]`
{:#members:disableditemindex}




Disables the given tab headers and content panels.


#### Default Value




* []




#### Example

{% highlight html %}

<ej-tab id="tab" [disabledItemIndex]="disabledItemIndex">
    <ul>
        <li><a href="#twitter">Twitter</a></li>
        <li><a href="#facebook">Facebook</a></li>
        <li><a href="#whatsapp">WhatsApp</a></li>
    </ul>
    <div id="twitter">
        Twitter is an online social networking service that enables users to send and read short 140-character messages called "tweets".
        Registered users can read and post tweets, but those who are unregistered can only read them. Users access Twitter through the website interface, SMS or mobile device app Twitter Inc. is based in San Francisco and has more than 25 offices around the world.
        Twitter was created in March 2006 by Jack Dorsey, Evan Williams, Biz Stone, and Noah Glass and launched in July 2006. The service rapidly gained worldwide popularity, with more than 100 million users posting 340 million tweets a day in 2012.The service also handled 1.6 billion search queries per day.
    </div>
    <div id="facebook">
        Facebook is an online social networking service headquartered in Menlo Park, California. Its website was launched on February 4, 2004, by Mark Zuckerberg with his Harvard College roommates and fellow students Eduardo Saverin, Andrew McCollum, Dustin Moskovitz and Chris Hughes.The founders had initially limited the website's membership to Harvard students, but later expanded it to colleges in the Boston area, the Ivy League, and Stanford University. It gradually added support for students at various other universities and later to high-school students.
    </div>
    <div id="whatsapp">
        WhatsApp Messenger is a proprietary cross-platform instant messaging client for smart phones that operates under a subscription business model. It uses the Internet to send text messages, images, video, user location and audio media messages to other users using standard cellular mobile numbers.
        As of February 2016, WhatsApp had a user base of up to one billion,[10] making it the most globally popular messaging application.
        WhatsApp Inc., based in Mountain View, California, was acquired by Facebook Inc. on February 19, 2014, for approximately US$19.3 billion.
    </div>
</ej-tab>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    disabledItemIndex: array;
    constructor() {
       this.disabledItemIndex = [1,2];
    }
}


{% endhighlight %}




### enableAnimation `boolean`
{:#members:enableanimation}




Specifies the animation behavior of the tab.


#### Default Value




* true




#### Example

{% highlight html %}

<ej-tab id="tab" [enableAnimation]=true>
    <ul>
        <li><a href="#twitter">Twitter</a></li>
        <li><a href="#facebook">Facebook</a></li>
        <li><a href="#whatsapp">WhatsApp</a></li>
    </ul>
    <div id="twitter">
        Twitter is an online social networking service that enables users to send and read short 140-character messages called "tweets".
        Registered users can read and post tweets, but those who are unregistered can only read them. Users access Twitter through the website interface, SMS or mobile device app Twitter Inc. is based in San Francisco and has more than 25 offices around the world.
        Twitter was created in March 2006 by Jack Dorsey, Evan Williams, Biz Stone, and Noah Glass and launched in July 2006. The service rapidly gained worldwide popularity, with more than 100 million users posting 340 million tweets a day in 2012.The service also handled 1.6 billion search queries per day.
    </div>
    <div id="facebook">
        Facebook is an online social networking service headquartered in Menlo Park, California. Its website was launched on February 4, 2004, by Mark Zuckerberg with his Harvard College roommates and fellow students Eduardo Saverin, Andrew McCollum, Dustin Moskovitz and Chris Hughes.The founders had initially limited the website's membership to Harvard students, but later expanded it to colleges in the Boston area, the Ivy League, and Stanford University. It gradually added support for students at various other universities and later to high-school students.
    </div>
    <div id="whatsapp">
        WhatsApp Messenger is a proprietary cross-platform instant messaging client for smart phones that operates under a subscription business model. It uses the Internet to send text messages, images, video, user location and audio media messages to other users using standard cellular mobile numbers.
        As of February 2016, WhatsApp had a user base of up to one billion,[10] making it the most globally popular messaging application.
        WhatsApp Inc., based in Mountain View, California, was acquired by Facebook Inc. on February 19, 2014, for approximately US$19.3 billion.
    </div>
</ej-tab>

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
}


{% endhighlight %}





### enabled `boolean`
{:#members:enabled}




When this property is set to false, it disables the tab control.


#### Default Value




* true




#### Example

{% highlight html %}

<ej-tab id="tab" [enabled]=true>
    <ul>
        <li><a href="#twitter">Twitter</a></li>
        <li><a href="#facebook">Facebook</a></li>
        <li><a href="#whatsapp">WhatsApp</a></li>
    </ul>
    <div id="twitter">
        Twitter is an online social networking service that enables users to send and read short 140-character messages called "tweets".
        Registered users can read and post tweets, but those who are unregistered can only read them. Users access Twitter through the website interface, SMS or mobile device app Twitter Inc. is based in San Francisco and has more than 25 offices around the world.
        Twitter was created in March 2006 by Jack Dorsey, Evan Williams, Biz Stone, and Noah Glass and launched in July 2006. The service rapidly gained worldwide popularity, with more than 100 million users posting 340 million tweets a day in 2012.The service also handled 1.6 billion search queries per day.
    </div>
    <div id="facebook">
        Facebook is an online social networking service headquartered in Menlo Park, California. Its website was launched on February 4, 2004, by Mark Zuckerberg with his Harvard College roommates and fellow students Eduardo Saverin, Andrew McCollum, Dustin Moskovitz and Chris Hughes.The founders had initially limited the website's membership to Harvard students, but later expanded it to colleges in the Boston area, the Ivy League, and Stanford University. It gradually added support for students at various other universities and later to high-school students.
    </div>
    <div id="whatsapp">
        WhatsApp Messenger is a proprietary cross-platform instant messaging client for smart phones that operates under a subscription business model. It uses the Internet to send text messages, images, video, user location and audio media messages to other users using standard cellular mobile numbers.
        As of February 2016, WhatsApp had a user base of up to one billion,[10] making it the most globally popular messaging application.
        WhatsApp Inc., based in Mountain View, California, was acquired by Facebook Inc. on February 19, 2014, for approximately US$19.3 billion.
    </div>
</ej-tab>

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
}


{% endhighlight %}







### enabledItemIndex `number[]`
{:#members:enableditemindex}




Enables the given tab headers and content panels.


#### Default Value




* []




#### Example

{% highlight html %}

<ej-tab id="tab" [enabledItemIndex]="enabledItemIndex" [disabledItemIndex]="disabledItemIndex">
    <ul>
        <li><a href="#twitter">Twitter</a></li>
        <li><a href="#facebook">Facebook</a></li>
        <li><a href="#whatsapp">WhatsApp</a></li>
    </ul>
    <div id="twitter">
        Twitter is an online social networking service that enables users to send and read short 140-character messages called "tweets".
        Registered users can read and post tweets, but those who are unregistered can only read them. Users access Twitter through the website interface, SMS or mobile device app Twitter Inc. is based in San Francisco and has more than 25 offices around the world.
        Twitter was created in March 2006 by Jack Dorsey, Evan Williams, Biz Stone, and Noah Glass and launched in July 2006. The service rapidly gained worldwide popularity, with more than 100 million users posting 340 million tweets a day in 2012.The service also handled 1.6 billion search queries per day.
    </div>
    <div id="facebook">
        Facebook is an online social networking service headquartered in Menlo Park, California. Its website was launched on February 4, 2004, by Mark Zuckerberg with his Harvard College roommates and fellow students Eduardo Saverin, Andrew McCollum, Dustin Moskovitz and Chris Hughes.The founders had initially limited the website's membership to Harvard students, but later expanded it to colleges in the Boston area, the Ivy League, and Stanford University. It gradually added support for students at various other universities and later to high-school students.
    </div>
    <div id="whatsapp">
        WhatsApp Messenger is a proprietary cross-platform instant messaging client for smart phones that operates under a subscription business model. It uses the Internet to send text messages, images, video, user location and audio media messages to other users using standard cellular mobile numbers.
        As of February 2016, WhatsApp had a user base of up to one billion,[10] making it the most globally popular messaging application.
        WhatsApp Inc., based in Mountain View, California, was acquired by Facebook Inc. on February 19, 2014, for approximately US$19.3 billion.
    </div>
</ej-tab>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    enabledItemIndex: any;
    enabledItemIndex: any;
    constructor() {
       this.disabledItemIndex = [0,1];
       this.enabledItemIndex = [0,1];
    }
}


{% endhighlight %}









### enablePersistence `boolean`
{:#members:enablepersistence}




Save current model value to browser cookies for state maintains. While refresh the Tab control page the model value apply from browser cookies.


#### Default Value




* false




#### Example

{% highlight html %}

<ej-tab id="tab" [enablePersistence]=true>
    <ul>
        <li><a href="#twitter">Twitter</a></li>
        <li><a href="#facebook">Facebook</a></li>
        <li><a href="#whatsapp">WhatsApp</a></li>
    </ul>
    <div id="twitter">
        Twitter is an online social networking service that enables users to send and read short 140-character messages called "tweets".
        Registered users can read and post tweets, but those who are unregistered can only read them. Users access Twitter through the website interface, SMS or mobile device app Twitter Inc. is based in San Francisco and has more than 25 offices around the world.
        Twitter was created in March 2006 by Jack Dorsey, Evan Williams, Biz Stone, and Noah Glass and launched in July 2006. The service rapidly gained worldwide popularity, with more than 100 million users posting 340 million tweets a day in 2012.The service also handled 1.6 billion search queries per day.
    </div>
    <div id="facebook">
        Facebook is an online social networking service headquartered in Menlo Park, California. Its website was launched on February 4, 2004, by Mark Zuckerberg with his Harvard College roommates and fellow students Eduardo Saverin, Andrew McCollum, Dustin Moskovitz and Chris Hughes.The founders had initially limited the website's membership to Harvard students, but later expanded it to colleges in the Boston area, the Ivy League, and Stanford University. It gradually added support for students at various other universities and later to high-school students.
    </div>
    <div id="whatsapp">
        WhatsApp Messenger is a proprietary cross-platform instant messaging client for smart phones that operates under a subscription business model. It uses the Internet to send text messages, images, video, user location and audio media messages to other users using standard cellular mobile numbers.
        As of February 2016, WhatsApp had a user base of up to one billion,[10] making it the most globally popular messaging application.
        WhatsApp Inc., based in Mountain View, California, was acquired by Facebook Inc. on February 19, 2014, for approximately US$19.3 billion.
    </div>
</ej-tab>

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
}


{% endhighlight %}







### enableRTL `boolean`
{:#members:enablertl}




Display Right to Left direction for headers and panels text of tab.


#### Default Value




* false




#### Example

{% highlight html %}

<ej-tab id="tab" [enableRTL]=true>
    <ul>
        <li><a href="#twitter">Twitter</a></li>
        <li><a href="#facebook">Facebook</a></li>
        <li><a href="#whatsapp">WhatsApp</a></li>
    </ul>
    <div id="twitter">
        Twitter is an online social networking service that enables users to send and read short 140-character messages called "tweets".
        Registered users can read and post tweets, but those who are unregistered can only read them. Users access Twitter through the website interface, SMS or mobile device app Twitter Inc. is based in San Francisco and has more than 25 offices around the world.
        Twitter was created in March 2006 by Jack Dorsey, Evan Williams, Biz Stone, and Noah Glass and launched in July 2006. The service rapidly gained worldwide popularity, with more than 100 million users posting 340 million tweets a day in 2012.The service also handled 1.6 billion search queries per day.
    </div>
    <div id="facebook">
        Facebook is an online social networking service headquartered in Menlo Park, California. Its website was launched on February 4, 2004, by Mark Zuckerberg with his Harvard College roommates and fellow students Eduardo Saverin, Andrew McCollum, Dustin Moskovitz and Chris Hughes.The founders had initially limited the website's membership to Harvard students, but later expanded it to colleges in the Boston area, the Ivy League, and Stanford University. It gradually added support for students at various other universities and later to high-school students.
    </div>
    <div id="whatsapp">
        WhatsApp Messenger is a proprietary cross-platform instant messaging client for smart phones that operates under a subscription business model. It uses the Internet to send text messages, images, video, user location and audio media messages to other users using standard cellular mobile numbers.
        As of February 2016, WhatsApp had a user base of up to one billion,[10] making it the most globally popular messaging application.
        WhatsApp Inc., based in Mountain View, California, was acquired by Facebook Inc. on February 19, 2014, for approximately US$19.3 billion.
    </div>
</ej-tab>

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
}


{% endhighlight %}






### enableTabScroll `boolean`
{:#members:enabletabscroll}




Specify to enable scrolling for Tab header.


#### Default Value




* false




#### Example

{% highlight ts %}

<<div style="width:600px; margin-left: 25%">
<ej-tab id="scrollTab" [enableTabScroll]="enableTabScroll" style='display: block'>
        <ul>
            <li><a href="#pizza">Pizza Menu</a></li>
            <li><a href="#pasta">Pasta Menu</a></li>
            <li><a href="#burger">Burger Menu</a></li>
            <li><a href="#sandwich">Sandwich Menu</a></li>
            <li><a href="#spaghetti">Spaghetti Menu</a></li>
            <li><a href="#ramen">Ramen Menu</a></li>
        </ul>
        <div id="pizza" style="background-color: #F5F5F5">
            <!--Food item description-->
            <p>
                Pizza cooked to perfection tossed with milk, vegetables, potatoes, poultry, 100% pure mutton, and cheese - and in creating nutritious and tasty meals to maintain good health.</p>
        </div>
        <div id="pasta" style="background-color: #F5F5F5">
            <!--dish description-->
            <p>
                Pasta cooked to perfection tossed with bread, milk, vegetables, potatoes, poultry, 100% pure mutton, and cheese - and in creating nutritious and tasty meals to maintain good health.</p>
        </div>
        <div id="sandwich" style="background-color: #F5F5F5">
            <!--dish description-->
            <p>
                Sandwich cooked to perfection tossed with bread, milk, vegetables, potatoes, poultry, 100% pure mutton, and cheese - and in creating nutritious and tasty meals to maintain good health.</p>
        </div>
        <div id="burger" style="background-color: #F5F5F5">
            <!--dish description-->
            <p>
                Burger cooked to perfection tossed with bread, milk, vegetables, potatoes, poultry, 100% pure mutton, and cheese - and in creating nutritious and tasty meals to maintain good health.</p>
        </div>
        <div id="spaghetti" style="background-color: #F5F5F5">
            <!--dish description-->
            <p>
                Spaghetti cooked to perfection tossed with bread, milk, vegetables, potatoes, poultry, 100% pure mutton, and cheese - and in creating nutritious and tasty meals to maintain good health.</p>
        </div>
        <div id="ramen" style="background-color: #F5F5F5">
            <!--dish description-->
            <p>
                Ramen cooked to perfection tossed with bread, milk, vegetables, potatoes, poultry, 100% pure mutton, and cheese - and in creating nutritious and tasty meals to maintain good health.</p>
        </div>
    </ej-tab>
</div>


{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './tab.component.html',
    styleUrls: ['./tab.component.css'],
    encapsulation: ViewEncapsulation.None,
})
export class ScrollTabComponent {
    enableTabScroll:boolean;
    constructor() {
    this.enableTabScroll=true;
    }
}



{% endhighlight %}




### events `string`
{:#members:events}




The event API to bind the action for active the tab items.


#### Default Value




* "click"




#### Example

{% highlight html %}

<ej-tab id="tab" events="click">
    <ul>
        <li><a href="#twitter">Twitter</a></li>
        <li><a href="#facebook">Facebook</a></li>
        <li><a href="#whatsapp">WhatsApp</a></li>
    </ul>
    <div id="twitter">
        Twitter is an online social networking service that enables users to send and read short 140-character messages called "tweets".
        Registered users can read and post tweets, but those who are unregistered can only read them. Users access Twitter through the website interface, SMS or mobile device app Twitter Inc. is based in San Francisco and has more than 25 offices around the world.
        Twitter was created in March 2006 by Jack Dorsey, Evan Williams, Biz Stone, and Noah Glass and launched in July 2006. The service rapidly gained worldwide popularity, with more than 100 million users posting 340 million tweets a day in 2012.The service also handled 1.6 billion search queries per day.
    </div>
    <div id="facebook">
        Facebook is an online social networking service headquartered in Menlo Park, California. Its website was launched on February 4, 2004, by Mark Zuckerberg with his Harvard College roommates and fellow students Eduardo Saverin, Andrew McCollum, Dustin Moskovitz and Chris Hughes.The founders had initially limited the website's membership to Harvard students, but later expanded it to colleges in the Boston area, the Ivy League, and Stanford University. It gradually added support for students at various other universities and later to high-school students.
    </div>
    <div id="whatsapp">
        WhatsApp Messenger is a proprietary cross-platform instant messaging client for smart phones that operates under a subscription business model. It uses the Internet to send text messages, images, video, user location and audio media messages to other users using standard cellular mobile numbers.
        As of February 2016, WhatsApp had a user base of up to one billion,[10] making it the most globally popular messaging application.
        WhatsApp Inc., based in Mountain View, California, was acquired by Facebook Inc. on February 19, 2014, for approximately US$19.3 billion.
    </div>
</ej-tab>

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
}


{% endhighlight %}




### headerPosition `string | enum`
{:#members:headerposition}


<ts name="ej.Tab.Position"/>

Specifies the position of Tab header as top, bottom, left or right. See below to get available Position

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
Top</td>
<td class="description">Tab headers display to top position</td>
</tr>
<tr>
<td class="name">
Bottom</td>
<td class="description">Tab headers display to bottom position </td>
</tr>
<tr>
<td class="name">
Left</td>
<td class="description">Tab headers display to left position.</td>
</tr>
<tr>
<td class="name">
Right</td>
<td class="description">Tab headers display to right position.</td>
</tr>

</tbody>
</table>


#### Default Value




* "top"




#### Example

{% highlight html %}

<ej-tab id="tab" headerPosition="left">
    <ul>
        <li><a href="#twitter">Twitter</a></li>
        <li><a href="#facebook">Facebook</a></li>
        <li><a href="#whatsapp">WhatsApp</a></li>
    </ul>
    <div id="twitter">
        Twitter is an online social networking service that enables users to send and read short 140-character messages called "tweets".
        Registered users can read and post tweets, but those who are unregistered can only read them. Users access Twitter through the website interface, SMS or mobile device app Twitter Inc. is based in San Francisco and has more than 25 offices around the world.
        Twitter was created in March 2006 by Jack Dorsey, Evan Williams, Biz Stone, and Noah Glass and launched in July 2006. The service rapidly gained worldwide popularity, with more than 100 million users posting 340 million tweets a day in 2012.The service also handled 1.6 billion search queries per day.
    </div>
    <div id="facebook">
        Facebook is an online social networking service headquartered in Menlo Park, California. Its website was launched on February 4, 2004, by Mark Zuckerberg with his Harvard College roommates and fellow students Eduardo Saverin, Andrew McCollum, Dustin Moskovitz and Chris Hughes.The founders had initially limited the website's membership to Harvard students, but later expanded it to colleges in the Boston area, the Ivy League, and Stanford University. It gradually added support for students at various other universities and later to high-school students.
    </div>
    <div id="whatsapp">
        WhatsApp Messenger is a proprietary cross-platform instant messaging client for smart phones that operates under a subscription business model. It uses the Internet to send text messages, images, video, user location and audio media messages to other users using standard cellular mobile numbers.
        As of February 2016, WhatsApp had a user base of up to one billion,[10] making it the most globally popular messaging application.
        WhatsApp Inc., based in Mountain View, California, was acquired by Facebook Inc. on February 19, 2014, for approximately US$19.3 billion.
    </div>
</ej-tab>

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
}


{% endhighlight %}





### headerSize `string | number`
{:#members:headersize}




Set the height of the tab header element. Default this property value is null, so height take content height.


#### Default Value




* null




#### Example

{% highlight html %}

<ej-tab id="tab" headerSize="100px">
    <ul>
        <li><a href="#twitter">Twitter</a></li>
        <li><a href="#facebook">Facebook</a></li>
        <li><a href="#whatsapp">WhatsApp</a></li>
    </ul>
    <div id="twitter">
        Twitter is an online social networking service that enables users to send and read short 140-character messages called "tweets".
        Registered users can read and post tweets, but those who are unregistered can only read them. Users access Twitter through the website interface, SMS or mobile device app Twitter Inc. is based in San Francisco and has more than 25 offices around the world.
        Twitter was created in March 2006 by Jack Dorsey, Evan Williams, Biz Stone, and Noah Glass and launched in July 2006. The service rapidly gained worldwide popularity, with more than 100 million users posting 340 million tweets a day in 2012.The service also handled 1.6 billion search queries per day.
    </div>
    <div id="facebook">
        Facebook is an online social networking service headquartered in Menlo Park, California. Its website was launched on February 4, 2004, by Mark Zuckerberg with his Harvard College roommates and fellow students Eduardo Saverin, Andrew McCollum, Dustin Moskovitz and Chris Hughes.The founders had initially limited the website's membership to Harvard students, but later expanded it to colleges in the Boston area, the Ivy League, and Stanford University. It gradually added support for students at various other universities and later to high-school students.
    </div>
    <div id="whatsapp">
        WhatsApp Messenger is a proprietary cross-platform instant messaging client for smart phones that operates under a subscription business model. It uses the Internet to send text messages, images, video, user location and audio media messages to other users using standard cellular mobile numbers.
        As of February 2016, WhatsApp had a user base of up to one billion,[10] making it the most globally popular messaging application.
        WhatsApp Inc., based in Mountain View, California, was acquired by Facebook Inc. on February 19, 2014, for approximately US$19.3 billion.
    </div>
</ej-tab>

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
}


{% endhighlight %}





### height `string | number`
{:#members:height}




Height set the outer panel element. Default this property value is null, so height take content height.


#### Default Value




* null




#### Example

{% highlight html %}

<ej-tab id="tab" height="320">
    <ul>
        <li><a href="#twitter">Twitter</a></li>
        <li><a href="#facebook">Facebook</a></li>
        <li><a href="#whatsapp">WhatsApp</a></li>
    </ul>
    <div id="twitter">
        Twitter is an online social networking service that enables users to send and read short 140-character messages called "tweets".
        Registered users can read and post tweets, but those who are unregistered can only read them. Users access Twitter through the website interface, SMS or mobile device app Twitter Inc. is based in San Francisco and has more than 25 offices around the world.
        Twitter was created in March 2006 by Jack Dorsey, Evan Williams, Biz Stone, and Noah Glass and launched in July 2006. The service rapidly gained worldwide popularity, with more than 100 million users posting 340 million tweets a day in 2012.The service also handled 1.6 billion search queries per day.
    </div>
    <div id="facebook">
        Facebook is an online social networking service headquartered in Menlo Park, California. Its website was launched on February 4, 2004, by Mark Zuckerberg with his Harvard College roommates and fellow students Eduardo Saverin, Andrew McCollum, Dustin Moskovitz and Chris Hughes.The founders had initially limited the website's membership to Harvard students, but later expanded it to colleges in the Boston area, the Ivy League, and Stanford University. It gradually added support for students at various other universities and later to high-school students.
    </div>
    <div id="whatsapp">
        WhatsApp Messenger is a proprietary cross-platform instant messaging client for smart phones that operates under a subscription business model. It uses the Internet to send text messages, images, video, user location and audio media messages to other users using standard cellular mobile numbers.
        As of February 2016, WhatsApp had a user base of up to one billion,[10] making it the most globally popular messaging application.
        WhatsApp Inc., based in Mountain View, California, was acquired by Facebook Inc. on February 19, 2014, for approximately US$19.3 billion.
    </div>
</ej-tab>

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
}


{% endhighlight %}




### heightAdjustMode `string | enum`
{:#members:heightadjustmode}

<ts name="ej.Tab.HeightAdjustMode"/>


Adjust the content panel height for given option (content, auto and fill), by default panels height adjust based on the content.See below to get available HeightAdjustMode

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
None</td>
<td class="type">string</td>
<td class="default">content</td>
<td class="description">Content panel take based on the height property.</td>
</tr>
<tr>
<td class="name">
Content</td>
<td class="type">string</td>
<td class="default">content</td>
<td class="description">Content panel will take height based on the content height.</td>
</tr>
<tr>
<td class="name">
Auto</td>
<td class="type">string</td>
<td class="default">auto</td>
<td class="description">All panel height will be set the tallest panel height</td>
</tr>
<tr>
<td class="name">
Fill</td>
<td class="type">string</td>
<td class="default">fill</td>
<td class="description">Content panel take based on the parent height</td>
</tr>
</tbody>
</table>

#### Default Value




* "content"




#### Example

{% highlight html %}

<ej-tab id="tab" heightAdjustMode="context">
    <ul>
        <li><a href="#twitter">Twitter</a></li>
        <li><a href="#facebook">Facebook</a></li>
        <li><a href="#whatsapp">WhatsApp</a></li>
    </ul>
    <div id="twitter">
        Twitter is an online social networking service that enables users to send and read short 140-character messages called "tweets".
        Registered users can read and post tweets, but those who are unregistered can only read them. Users access Twitter through the website interface, SMS or mobile device app Twitter Inc. is based in San Francisco and has more than 25 offices around the world.
        Twitter was created in March 2006 by Jack Dorsey, Evan Williams, Biz Stone, and Noah Glass and launched in July 2006. The service rapidly gained worldwide popularity, with more than 100 million users posting 340 million tweets a day in 2012.The service also handled 1.6 billion search queries per day.
    </div>
    <div id="facebook">
        Facebook is an online social networking service headquartered in Menlo Park, California. Its website was launched on February 4, 2004, by Mark Zuckerberg with his Harvard College roommates and fellow students Eduardo Saverin, Andrew McCollum, Dustin Moskovitz and Chris Hughes.The founders had initially limited the website's membership to Harvard students, but later expanded it to colleges in the Boston area, the Ivy League, and Stanford University. It gradually added support for students at various other universities and later to high-school students.
    </div>
    <div id="whatsapp">
        WhatsApp Messenger is a proprietary cross-platform instant messaging client for smart phones that operates under a subscription business model. It uses the Internet to send text messages, images, video, user location and audio media messages to other users using standard cellular mobile numbers.
        As of February 2016, WhatsApp had a user base of up to one billion,[10] making it the most globally popular messaging application.
        WhatsApp Inc., based in Mountain View, California, was acquired by Facebook Inc. on February 19, 2014, for approximately US$19.3 billion.
    </div>
</ej-tab>

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
}


{% endhighlight %}








### hiddenItemIndex `array`
{:#members:hiddenitemindex}








Specifies to hide a pane of Tab control.





#### Default Value







* []








#### Example

{% highlight html %}

<ej-tab id="tab" [hiddenItemIndex]="hiddenItemIndex">
    
    <ul>
        <li><a href="#twitter">Twitter</a></li>
        <li><a href="#facebook">Facebook</a></li>
        <li><a href="#whatsapp">WhatsApp</a></li>
    </ul>
    <div id="twitter">
        Twitter is an online social networking service that enables users to send and read short 140-character messages called "tweets".
        Registered users can read and post tweets, but those who are unregistered can only read them. Users access Twitter through the website interface, SMS or mobile device app Twitter Inc. is based in San Francisco and has more than 25 offices around the world.
        Twitter was created in March 2006 by Jack Dorsey, Evan Williams, Biz Stone, and Noah Glass and launched in July 2006. The service rapidly gained worldwide popularity, with more than 100 million users posting 340 million tweets a day in 2012.The service also handled 1.6 billion search queries per day.
    </div>
    <div id="facebook">
        Facebook is an online social networking service headquartered in Menlo Park, California. Its website was launched on February 4, 2004, by Mark Zuckerberg with his Harvard College roommates and fellow students Eduardo Saverin, Andrew McCollum, Dustin Moskovitz and Chris Hughes.The founders had initially limited the website's membership to Harvard students, but later expanded it to colleges in the Boston area, the Ivy League, and Stanford University. It gradually added support for students at various other universities and later to high-school students.
    </div>
    <div id="whatsapp">
        WhatsApp Messenger is a proprietary cross-platform instant messaging client for smart phones that operates under a subscription business model. It uses the Internet to send text messages, images, video, user location and audio media messages to other users using standard cellular mobile numbers.
        As of February 2016, WhatsApp had a user base of up to one billion,[10] making it the most globally popular messaging application.
        WhatsApp Inc., based in Mountain View, California, was acquired by Facebook Inc. on February 19, 2014, for approximately US$19.3 billion.
    </div>
</ej-tab>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    hiddenItemIndex: array;
    constructor() {
       this.hiddenItemIndex= [0,1];
    }
}


{% endhighlight %}








### htmlAttributes `object`
{:#members:htmlattributes}








Specifies the HTML Attributes of the Tab.





#### Default Value







* {}








#### Example

{% highlight html %}

<ej-tab id="tab" [htmlAttributes]="htmlAttributes">
    <ul>
        <li><a href="#twitter">Twitter</a></li>
        <li><a href="#facebook">Facebook</a></li>
        <li><a href="#whatsapp">WhatsApp</a></li>
    </ul>
    <div id="twitter">
        Twitter is an online social networking service that enables users to send and read short 140-character messages called "tweets".
        Registered users can read and post tweets, but those who are unregistered can only read them. Users access Twitter through the website interface, SMS or mobile device app Twitter Inc. is based in San Francisco and has more than 25 offices around the world.
        Twitter was created in March 2006 by Jack Dorsey, Evan Williams, Biz Stone, and Noah Glass and launched in July 2006. The service rapidly gained worldwide popularity, with more than 100 million users posting 340 million tweets a day in 2012.The service also handled 1.6 billion search queries per day.
    </div>
    <div id="facebook">
        Facebook is an online social networking service headquartered in Menlo Park, California. Its website was launched on February 4, 2004, by Mark Zuckerberg with his Harvard College roommates and fellow students Eduardo Saverin, Andrew McCollum, Dustin Moskovitz and Chris Hughes.The founders had initially limited the website's membership to Harvard students, but later expanded it to colleges in the Boston area, the Ivy League, and Stanford University. It gradually added support for students at various other universities and later to high-school students.
    </div>
    <div id="whatsapp">
        WhatsApp Messenger is a proprietary cross-platform instant messaging client for smart phones that operates under a subscription business model. It uses the Internet to send text messages, images, video, user location and audio media messages to other users using standard cellular mobile numbers.
        As of February 2016, WhatsApp had a user base of up to one billion,[10] making it the most globally popular messaging application.
        WhatsApp Inc., based in Mountain View, California, was acquired by Facebook Inc. on February 19, 2014, for approximately US$19.3 billion.
    </div>
</ej-tab>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    htmlAttributes: Object;
    constructor() {
       this.htmlAttributes = {class:"my-class"};
    }
}


{% endhighlight %}











### idPrefix `string`
{:#members:idprefix}




The idPrefix property appends the given string on the added tab item id&rsquo;s in runtime.


#### Default Value




* "ej-tab-"




#### Example

{% highlight html %}

<ej-tab id="tab" [allowKeyboardNavigation]=true>
    <ul>
        <li><a href="#twitter">Twitter</a></li>
        <li><a href="#facebook">Facebook</a></li>
        <li><a href="#whatsapp">WhatsApp</a></li>
    </ul>
    <div id="twitter">
        Twitter is an online social networking service that enables users to send and read short 140-character messages called "tweets".
        Registered users can read and post tweets, but those who are unregistered can only read them. Users access Twitter through the website interface, SMS or mobile device app Twitter Inc. is based in San Francisco and has more than 25 offices around the world.
        Twitter was created in March 2006 by Jack Dorsey, Evan Williams, Biz Stone, and Noah Glass and launched in July 2006. The service rapidly gained worldwide popularity, with more than 100 million users posting 340 million tweets a day in 2012.The service also handled 1.6 billion search queries per day.
    </div>
    <div id="facebook">
        Facebook is an online social networking service headquartered in Menlo Park, California. Its website was launched on February 4, 2004, by Mark Zuckerberg with his Harvard College roommates and fellow students Eduardo Saverin, Andrew McCollum, Dustin Moskovitz and Chris Hughes.The founders had initially limited the website's membership to Harvard students, but later expanded it to colleges in the Boston area, the Ivy League, and Stanford University. It gradually added support for students at various other universities and later to high-school students.
    </div>
    <div id="whatsapp">
        WhatsApp Messenger is a proprietary cross-platform instant messaging client for smart phones that operates under a subscription business model. It uses the Internet to send text messages, images, video, user location and audio media messages to other users using standard cellular mobile numbers.
        As of February 2016, WhatsApp had a user base of up to one billion,[10] making it the most globally popular messaging application.
        WhatsApp Inc., based in Mountain View, California, was acquired by Facebook Inc. on February 19, 2014, for approximately US$19.3 billion.
    </div>
</ej-tab>

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
}


{% endhighlight %}





### selectedItemIndex `number`
{:#members:selecteditemindex}




Specifies the Tab header in active for given index value.


#### Default Value




* 0




#### Example

{% highlight html %}

<ej-tab id="tab" [selectedItemIndex]="selectedItemIndex">
    <ul>
        <li><a href="#twitter">Twitter</a></li>
        <li><a href="#facebook">Facebook</a></li>
        <li><a href="#whatsapp">WhatsApp</a></li>
    </ul>
    <div id="twitter">
        Twitter is an online social networking service that enables users to send and read short 140-character messages called "tweets".
        Registered users can read and post tweets, but those who are unregistered can only read them. Users access Twitter through the website interface, SMS or mobile device app Twitter Inc. is based in San Francisco and has more than 25 offices around the world.
        Twitter was created in March 2006 by Jack Dorsey, Evan Williams, Biz Stone, and Noah Glass and launched in July 2006. The service rapidly gained worldwide popularity, with more than 100 million users posting 340 million tweets a day in 2012.The service also handled 1.6 billion search queries per day.
    </div>
    <div id="facebook">
        Facebook is an online social networking service headquartered in Menlo Park, California. Its website was launched on February 4, 2004, by Mark Zuckerberg with his Harvard College roommates and fellow students Eduardo Saverin, Andrew McCollum, Dustin Moskovitz and Chris Hughes.The founders had initially limited the website's membership to Harvard students, but later expanded it to colleges in the Boston area, the Ivy League, and Stanford University. It gradually added support for students at various other universities and later to high-school students.
    </div>
    <div id="whatsapp">
        WhatsApp Messenger is a proprietary cross-platform instant messaging client for smart phones that operates under a subscription business model. It uses the Internet to send text messages, images, video, user location and audio media messages to other users using standard cellular mobile numbers.
        As of February 2016, WhatsApp had a user base of up to one billion,[10] making it the most globally popular messaging application.
        WhatsApp Inc., based in Mountain View, California, was acquired by Facebook Inc. on February 19, 2014, for approximately US$19.3 billion.
    </div>
</ej-tab>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
     selectedItemIndex: any;
    constructor() {
       this.selectedItemIndex = 1;
    }
}


{% endhighlight %}





### showCloseButton `boolean`
{:#members:showclosebutton}




Display the close button for each tab items. While clicking on the close icon, particular tab item will be removed.


#### Default Value




* false




#### Example

{% highlight html %}

<ej-tab id="tab" [showCloseButton]=true>
    <ul>
        <li><a href="#twitter">Twitter</a></li>
        <li><a href="#facebook">Facebook</a></li>
        <li><a href="#whatsapp">WhatsApp</a></li>
    </ul>
    <div id="twitter">
        Twitter is an online social networking service that enables users to send and read short 140-character messages called "tweets".
        Registered users can read and post tweets, but those who are unregistered can only read them. Users access Twitter through the website interface, SMS or mobile device app Twitter Inc. is based in San Francisco and has more than 25 offices around the world.
        Twitter was created in March 2006 by Jack Dorsey, Evan Williams, Biz Stone, and Noah Glass and launched in July 2006. The service rapidly gained worldwide popularity, with more than 100 million users posting 340 million tweets a day in 2012.The service also handled 1.6 billion search queries per day.
    </div>
    <div id="facebook">
        Facebook is an online social networking service headquartered in Menlo Park, California. Its website was launched on February 4, 2004, by Mark Zuckerberg with his Harvard College roommates and fellow students Eduardo Saverin, Andrew McCollum, Dustin Moskovitz and Chris Hughes.The founders had initially limited the website's membership to Harvard students, but later expanded it to colleges in the Boston area, the Ivy League, and Stanford University. It gradually added support for students at various other universities and later to high-school students.
    </div>
    <div id="whatsapp">
        WhatsApp Messenger is a proprietary cross-platform instant messaging client for smart phones that operates under a subscription business model. It uses the Internet to send text messages, images, video, user location and audio media messages to other users using standard cellular mobile numbers.
        As of February 2016, WhatsApp had a user base of up to one billion,[10] making it the most globally popular messaging application.
        WhatsApp Inc., based in Mountain View, California, was acquired by Facebook Inc. on February 19, 2014, for approximately US$19.3 billion.
    </div>
</ej-tab>

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
}


{% endhighlight %}




### showReloadIcon `boolean`
{:#members:showreloadicon}




Display the Reload button for each tab items.


#### Default Value




* false




#### Example

{% highlight html %}

<ej-tab id="tab" [showReloadIcon]=true>
    <ul>
        <li><a href="#twitter">Twitter</a></li>
        <li><a href="#facebook">Facebook</a></li>
        <li><a href="#whatsapp">WhatsApp</a></li>
    </ul>
    <div id="twitter">
        Twitter is an online social networking service that enables users to send and read short 140-character messages called "tweets".
        Registered users can read and post tweets, but those who are unregistered can only read them. Users access Twitter through the website interface, SMS or mobile device app Twitter Inc. is based in San Francisco and has more than 25 offices around the world.
        Twitter was created in March 2006 by Jack Dorsey, Evan Williams, Biz Stone, and Noah Glass and launched in July 2006. The service rapidly gained worldwide popularity, with more than 100 million users posting 340 million tweets a day in 2012.The service also handled 1.6 billion search queries per day.
    </div>
    <div id="facebook">
        Facebook is an online social networking service headquartered in Menlo Park, California. Its website was launched on February 4, 2004, by Mark Zuckerberg with his Harvard College roommates and fellow students Eduardo Saverin, Andrew McCollum, Dustin Moskovitz and Chris Hughes.The founders had initially limited the website's membership to Harvard students, but later expanded it to colleges in the Boston area, the Ivy League, and Stanford University. It gradually added support for students at various other universities and later to high-school students.
    </div>
    <div id="whatsapp">
        WhatsApp Messenger is a proprietary cross-platform instant messaging client for smart phones that operates under a subscription business model. It uses the Internet to send text messages, images, video, user location and audio media messages to other users using standard cellular mobile numbers.
        As of February 2016, WhatsApp had a user base of up to one billion,[10] making it the most globally popular messaging application.
        WhatsApp Inc., based in Mountain View, California, was acquired by Facebook Inc. on February 19, 2014, for approximately US$19.3 billion.
    </div>
</ej-tab>

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
}


{% endhighlight %}





### showRoundedCorner `boolean`
{:#members:showroundedcorner}




Tab panels and headers to be displayed in rounded corner style.


#### Default Value




* false




#### Example

{% highlight html %}

<ej-tab id="tab" [showRoundedCorner]=true>
    <ul>
        <li><a href="#twitter">Twitter</a></li>
        <li><a href="#facebook">Facebook</a></li>
        <li><a href="#whatsapp">WhatsApp</a></li>
    </ul>
    <div id="twitter">
        Twitter is an online social networking service that enables users to send and read short 140-character messages called "tweets".
        Registered users can read and post tweets, but those who are unregistered can only read them. Users access Twitter through the website interface, SMS or mobile device app Twitter Inc. is based in San Francisco and has more than 25 offices around the world.
        Twitter was created in March 2006 by Jack Dorsey, Evan Williams, Biz Stone, and Noah Glass and launched in July 2006. The service rapidly gained worldwide popularity, with more than 100 million users posting 340 million tweets a day in 2012.The service also handled 1.6 billion search queries per day.
    </div>
    <div id="facebook">
        Facebook is an online social networking service headquartered in Menlo Park, California. Its website was launched on February 4, 2004, by Mark Zuckerberg with his Harvard College roommates and fellow students Eduardo Saverin, Andrew McCollum, Dustin Moskovitz and Chris Hughes.The founders had initially limited the website's membership to Harvard students, but later expanded it to colleges in the Boston area, the Ivy League, and Stanford University. It gradually added support for students at various other universities and later to high-school students.
    </div>
    <div id="whatsapp">
        WhatsApp Messenger is a proprietary cross-platform instant messaging client for smart phones that operates under a subscription business model. It uses the Internet to send text messages, images, video, user location and audio media messages to other users using standard cellular mobile numbers.
        As of February 2016, WhatsApp had a user base of up to one billion,[10] making it the most globally popular messaging application.
        WhatsApp Inc., based in Mountain View, California, was acquired by Facebook Inc. on February 19, 2014, for approximately US$19.3 billion.
    </div>
</ej-tab>

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
}


{% endhighlight %}




### width `string | number`
{:#members:width}




Set the width for outer panel element, if not it&rsquo;s take parent width.


#### Default Value




* null




#### Example

{% highlight html %}

<ej-tab id="tab" width="300">
    <ul>
        <li><a href="#twitter">Twitter</a></li>
        <li><a href="#facebook">Facebook</a></li>
        <li><a href="#whatsapp">WhatsApp</a></li>
    </ul>
    <div id="twitter">
        Twitter is an online social networking service that enables users to send and read short 140-character messages called "tweets".
        Registered users can read and post tweets, but those who are unregistered can only read them. Users access Twitter through the website interface, SMS or mobile device app Twitter Inc. is based in San Francisco and has more than 25 offices around the world.
        Twitter was created in March 2006 by Jack Dorsey, Evan Williams, Biz Stone, and Noah Glass and launched in July 2006. The service rapidly gained worldwide popularity, with more than 100 million users posting 340 million tweets a day in 2012.The service also handled 1.6 billion search queries per day.
    </div>
    <div id="facebook">
        Facebook is an online social networking service headquartered in Menlo Park, California. Its website was launched on February 4, 2004, by Mark Zuckerberg with his Harvard College roommates and fellow students Eduardo Saverin, Andrew McCollum, Dustin Moskovitz and Chris Hughes.The founders had initially limited the website's membership to Harvard students, but later expanded it to colleges in the Boston area, the Ivy League, and Stanford University. It gradually added support for students at various other universities and later to high-school students.
    </div>
    <div id="whatsapp">
        WhatsApp Messenger is a proprietary cross-platform instant messaging client for smart phones that operates under a subscription business model. It uses the Internet to send text messages, images, video, user location and audio media messages to other users using standard cellular mobile numbers.
        As of February 2016, WhatsApp had a user base of up to one billion,[10] making it the most globally popular messaging application.
        WhatsApp Inc., based in Mountain View, California, was acquired by Facebook Inc. on February 19, 2014, for approximately US$19.3 billion.
    </div>
</ej-tab>

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
}


{% endhighlight %}



## Methods




### addItem(url, displayLabel, index, cssClass, id)
{:#methods:additem}




Add new tab items with given name, URL and given index position, if index null it&rsquo;s add last item.

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
URL</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">URL name / tab id.</td>
</tr>
<tr>
<td class="name">
displayLabel</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Tab Display name.</td>
</tr>
<tr>
<td class="name">
index</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Index position to placed , this is optional.</td>
</tr>
<tr>
<td class="name">
cssClass</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">specifies cssClass, this is optional.</td>
</tr>
<tr>
<td class="name">
id</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">specifies id of tab, this is optional.</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<ej-tab id="tab" [allowKeyboardNavigation]=true>
    <ul>
        <li><a href="#twitter">Twitter</a></li>
        <li><a href="#facebook">Facebook</a></li>
        <li><a href="#whatsapp">WhatsApp</a></li>
    </ul>
    <div id="twitter">
        Twitter is an online social networking service that enables users to send and read short 140-character messages called "tweets".
        Registered users can read and post tweets, but those who are unregistered can only read them. Users access Twitter through the website interface, SMS or mobile device app Twitter Inc. is based in San Francisco and has more than 25 offices around the world.
        Twitter was created in March 2006 by Jack Dorsey, Evan Williams, Biz Stone, and Noah Glass and launched in July 2006. The service rapidly gained worldwide popularity, with more than 100 million users posting 340 million tweets a day in 2012.The service also handled 1.6 billion search queries per day.
    </div>
    <div id="facebook">
        Facebook is an online social networking service headquartered in Menlo Park, California. Its website was launched on February 4, 2004, by Mark Zuckerberg with his Harvard College roommates and fellow students Eduardo Saverin, Andrew McCollum, Dustin Moskovitz and Chris Hughes.The founders had initially limited the website's membership to Harvard students, but later expanded it to colleges in the Boston area, the Ivy League, and Stanford University. It gradually added support for students at various other universities and later to high-school students.
    </div>
    <div id="whatsapp">
        WhatsApp Messenger is a proprietary cross-platform instant messaging client for smart phones that operates under a subscription business model. It uses the Internet to send text messages, images, video, user location and audio media messages to other users using standard cellular mobile numbers.
        As of February 2016, WhatsApp had a user base of up to one billion,[10] making it the most globally popular messaging application.
        WhatsApp Inc., based in Mountain View, California, was acquired by Facebook Inc. on February 19, 2014, for approximately US$19.3 billion.
    </div>
</ej-tab>
<button type="button" (click)="OnClick()">Add item</button>

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
    OnClick(){


var obj = $("#tab").data("ejTab");


obj.addItem("#new", "New Item", 3, "myClass", "newItem");

}
}


{% endhighlight %}

{% highlight html %}

<ej-tab id="tab" [allowKeyboardNavigation]=true>
    <ul>
        <li><a href="#twitter">Twitter</a></li>
        <li><a href="#facebook">Facebook</a></li>
        <li><a href="#whatsapp">WhatsApp</a></li>
    </ul>
    <div id="twitter">
        Twitter is an online social networking service that enables users to send and read short 140-character messages called "tweets".
        Registered users can read and post tweets, but those who are unregistered can only read them. Users access Twitter through the website interface, SMS or mobile device app Twitter Inc. is based in San Francisco and has more than 25 offices around the world.
        Twitter was created in March 2006 by Jack Dorsey, Evan Williams, Biz Stone, and Noah Glass and launched in July 2006. The service rapidly gained worldwide popularity, with more than 100 million users posting 340 million tweets a day in 2012.The service also handled 1.6 billion search queries per day.
    </div>
    <div id="facebook">
        Facebook is an online social networking service headquartered in Menlo Park, California. Its website was launched on February 4, 2004, by Mark Zuckerberg with his Harvard College roommates and fellow students Eduardo Saverin, Andrew McCollum, Dustin Moskovitz and Chris Hughes.The founders had initially limited the website's membership to Harvard students, but later expanded it to colleges in the Boston area, the Ivy League, and Stanford University. It gradually added support for students at various other universities and later to high-school students.
    </div>
    <div id="whatsapp">
        WhatsApp Messenger is a proprietary cross-platform instant messaging client for smart phones that operates under a subscription business model. It uses the Internet to send text messages, images, video, user location and audio media messages to other users using standard cellular mobile numbers.
        As of February 2016, WhatsApp had a user base of up to one billion,[10] making it the most globally popular messaging application.
        WhatsApp Inc., based in Mountain View, California, was acquired by Facebook Inc. on February 19, 2014, for approximately US$19.3 billion.
    </div>
</ej-tab>
<button type="button" (click)="OnClick()">Add item</button>

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
    OnClick(){

    $("#tab").ejTab("addItem","#new","New Item",3); 

}
}


{% endhighlight %}








### disable()
{:#methods:disable}




To disable the tab control.



#### Example

{% highlight html %}

<ej-tab id="tab" [allowKeyboardNavigation]=true>
    <ul>
        <li><a href="#twitter">Twitter</a></li>
        <li><a href="#facebook">Facebook</a></li>
        <li><a href="#whatsapp">WhatsApp</a></li>
    </ul>
    <div id="twitter">
        Twitter is an online social networking service that enables users to send and read short 140-character messages called "tweets".
        Registered users can read and post tweets, but those who are unregistered can only read them. Users access Twitter through the website interface, SMS or mobile device app Twitter Inc. is based in San Francisco and has more than 25 offices around the world.
        Twitter was created in March 2006 by Jack Dorsey, Evan Williams, Biz Stone, and Noah Glass and launched in July 2006. The service rapidly gained worldwide popularity, with more than 100 million users posting 340 million tweets a day in 2012.The service also handled 1.6 billion search queries per day.
    </div>
    <div id="facebook">
        Facebook is an online social networking service headquartered in Menlo Park, California. Its website was launched on February 4, 2004, by Mark Zuckerberg with his Harvard College roommates and fellow students Eduardo Saverin, Andrew McCollum, Dustin Moskovitz and Chris Hughes.The founders had initially limited the website's membership to Harvard students, but later expanded it to colleges in the Boston area, the Ivy League, and Stanford University. It gradually added support for students at various other universities and later to high-school students.
    </div>
    <div id="whatsapp">
        WhatsApp Messenger is a proprietary cross-platform instant messaging client for smart phones that operates under a subscription business model. It uses the Internet to send text messages, images, video, user location and audio media messages to other users using standard cellular mobile numbers.
        As of February 2016, WhatsApp had a user base of up to one billion,[10] making it the most globally popular messaging application.
        WhatsApp Inc., based in Mountain View, California, was acquired by Facebook Inc. on February 19, 2014, for approximately US$19.3 billion.
    </div>
</ej-tab>
<button type="button" (click)="OnClick()">Disable</button>

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
    OnClick(){


var obj = $("#tab").data("ejTab");


obj.disable();

}
}


{% endhighlight %}

{% highlight html %}

<ej-tab id="tab" [allowKeyboardNavigation]=true>
    <ul>
        <li><a href="#twitter">Twitter</a></li>
        <li><a href="#facebook">Facebook</a></li>
        <li><a href="#whatsapp">WhatsApp</a></li>
    </ul>
    <div id="twitter">
        Twitter is an online social networking service that enables users to send and read short 140-character messages called "tweets".
        Registered users can read and post tweets, but those who are unregistered can only read them. Users access Twitter through the website interface, SMS or mobile device app Twitter Inc. is based in San Francisco and has more than 25 offices around the world.
        Twitter was created in March 2006 by Jack Dorsey, Evan Williams, Biz Stone, and Noah Glass and launched in July 2006. The service rapidly gained worldwide popularity, with more than 100 million users posting 340 million tweets a day in 2012.The service also handled 1.6 billion search queries per day.
    </div>
    <div id="facebook">
        Facebook is an online social networking service headquartered in Menlo Park, California. Its website was launched on February 4, 2004, by Mark Zuckerberg with his Harvard College roommates and fellow students Eduardo Saverin, Andrew McCollum, Dustin Moskovitz and Chris Hughes.The founders had initially limited the website's membership to Harvard students, but later expanded it to colleges in the Boston area, the Ivy League, and Stanford University. It gradually added support for students at various other universities and later to high-school students.
    </div>
    <div id="whatsapp">
        WhatsApp Messenger is a proprietary cross-platform instant messaging client for smart phones that operates under a subscription business model. It uses the Internet to send text messages, images, video, user location and audio media messages to other users using standard cellular mobile numbers.
        As of February 2016, WhatsApp had a user base of up to one billion,[10] making it the most globally popular messaging application.
        WhatsApp Inc., based in Mountain View, California, was acquired by Facebook Inc. on February 19, 2014, for approximately US$19.3 billion.
    </div>
</ej-tab>
<button type="button" (click)="OnClick()">Disable</button>

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
    OnClick(){

    $("#tab").ejTab("disable"); 

}
}


{% endhighlight %}








### enable()
{:#methods:enable}




To enable the tab control.



#### Example

{% highlight html %}

<ej-tab id="tab" [allowKeyboardNavigation]=true [enabled]=false>
    <ul>
        <li><a href="#twitter">Twitter</a></li>
        <li><a href="#facebook">Facebook</a></li>
        <li><a href="#whatsapp">WhatsApp</a></li>
    </ul>
    <div id="twitter">
        Twitter is an online social networking service that enables users to send and read short 140-character messages called "tweets".
        Registered users can read and post tweets, but those who are unregistered can only read them. Users access Twitter through the website interface, SMS or mobile device app Twitter Inc. is based in San Francisco and has more than 25 offices around the world.
        Twitter was created in March 2006 by Jack Dorsey, Evan Williams, Biz Stone, and Noah Glass and launched in July 2006. The service rapidly gained worldwide popularity, with more than 100 million users posting 340 million tweets a day in 2012.The service also handled 1.6 billion search queries per day.
    </div>
    <div id="facebook">
        Facebook is an online social networking service headquartered in Menlo Park, California. Its website was launched on February 4, 2004, by Mark Zuckerberg with his Harvard College roommates and fellow students Eduardo Saverin, Andrew McCollum, Dustin Moskovitz and Chris Hughes.The founders had initially limited the website's membership to Harvard students, but later expanded it to colleges in the Boston area, the Ivy League, and Stanford University. It gradually added support for students at various other universities and later to high-school students.
    </div>
    <div id="whatsapp">
        WhatsApp Messenger is a proprietary cross-platform instant messaging client for smart phones that operates under a subscription business model. It uses the Internet to send text messages, images, video, user location and audio media messages to other users using standard cellular mobile numbers.
        As of February 2016, WhatsApp had a user base of up to one billion,[10] making it the most globally popular messaging application.
        WhatsApp Inc., based in Mountain View, California, was acquired by Facebook Inc. on February 19, 2014, for approximately US$19.3 billion.
    </div>
</ej-tab>
<button type="button" (click)="OnClick()">Enable</button>

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
    OnClick(){


var obj = $("#tab").data("ejTab");


obj.enable();

}
}


{% endhighlight %}

{% highlight html %}

<ej-tab id="tab" [allowKeyboardNavigation]=true [enabled]=false>
    <ul>
        <li><a href="#twitter">Twitter</a></li>
        <li><a href="#facebook">Facebook</a></li>
        <li><a href="#whatsapp">WhatsApp</a></li>
    </ul>
    <div id="twitter">
        Twitter is an online social networking service that enables users to send and read short 140-character messages called "tweets".
        Registered users can read and post tweets, but those who are unregistered can only read them. Users access Twitter through the website interface, SMS or mobile device app Twitter Inc. is based in San Francisco and has more than 25 offices around the world.
        Twitter was created in March 2006 by Jack Dorsey, Evan Williams, Biz Stone, and Noah Glass and launched in July 2006. The service rapidly gained worldwide popularity, with more than 100 million users posting 340 million tweets a day in 2012.The service also handled 1.6 billion search queries per day.
    </div>
    <div id="facebook">
        Facebook is an online social networking service headquartered in Menlo Park, California. Its website was launched on February 4, 2004, by Mark Zuckerberg with his Harvard College roommates and fellow students Eduardo Saverin, Andrew McCollum, Dustin Moskovitz and Chris Hughes.The founders had initially limited the website's membership to Harvard students, but later expanded it to colleges in the Boston area, the Ivy League, and Stanford University. It gradually added support for students at various other universities and later to high-school students.
    </div>
    <div id="whatsapp">
        WhatsApp Messenger is a proprietary cross-platform instant messaging client for smart phones that operates under a subscription business model. It uses the Internet to send text messages, images, video, user location and audio media messages to other users using standard cellular mobile numbers.
        As of February 2016, WhatsApp had a user base of up to one billion,[10] making it the most globally popular messaging application.
        WhatsApp Inc., based in Mountain View, California, was acquired by Facebook Inc. on February 19, 2014, for approximately US$19.3 billion.
    </div>
</ej-tab>
<button type="button" (click)="OnClick()">Enable</button>

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
    OnClick(){

    $("#tab").ejTab("enable"); 

}
}


{% endhighlight %}








### getItemsCount()
{:#methods:getitemscount}




This function get the number of tab rendered

####Returns

number

#### Example

{% highlight html %}

<ej-tab id="tab" [allowKeyboardNavigation]=true>
    <ul>
        <li><a href="#twitter">Twitter</a></li>
        <li><a href="#facebook">Facebook</a></li>
        <li><a href="#whatsapp">WhatsApp</a></li>
    </ul>
    <div id="twitter">
        Twitter is an online social networking service that enables users to send and read short 140-character messages called "tweets".
        Registered users can read and post tweets, but those who are unregistered can only read them. Users access Twitter through the website interface, SMS or mobile device app Twitter Inc. is based in San Francisco and has more than 25 offices around the world.
        Twitter was created in March 2006 by Jack Dorsey, Evan Williams, Biz Stone, and Noah Glass and launched in July 2006. The service rapidly gained worldwide popularity, with more than 100 million users posting 340 million tweets a day in 2012.The service also handled 1.6 billion search queries per day.
    </div>
    <div id="facebook">
        Facebook is an online social networking service headquartered in Menlo Park, California. Its website was launched on February 4, 2004, by Mark Zuckerberg with his Harvard College roommates and fellow students Eduardo Saverin, Andrew McCollum, Dustin Moskovitz and Chris Hughes.The founders had initially limited the website's membership to Harvard students, but later expanded it to colleges in the Boston area, the Ivy League, and Stanford University. It gradually added support for students at various other universities and later to high-school students.
    </div>
    <div id="whatsapp">
        WhatsApp Messenger is a proprietary cross-platform instant messaging client for smart phones that operates under a subscription business model. It uses the Internet to send text messages, images, video, user location and audio media messages to other users using standard cellular mobile numbers.
        As of February 2016, WhatsApp had a user base of up to one billion,[10] making it the most globally popular messaging application.
        WhatsApp Inc., based in Mountain View, California, was acquired by Facebook Inc. on February 19, 2014, for approximately US$19.3 billion.
    </div>
</ej-tab>
<button type="button" (click)="OnClick()">GetItemsCount</button>

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
    OnClick(){


var obj = $("#tab").data("ejTab");


obj.getItemsCount();

}
}


{% endhighlight %}

{% highlight html %}

<ej-tab id="tab" [allowKeyboardNavigation]=true>
    <ul>
        <li><a href="#twitter">Twitter</a></li>
        <li><a href="#facebook">Facebook</a></li>
        <li><a href="#whatsapp">WhatsApp</a></li>
    </ul>
    <div id="twitter">
        Twitter is an online social networking service that enables users to send and read short 140-character messages called "tweets".
        Registered users can read and post tweets, but those who are unregistered can only read them. Users access Twitter through the website interface, SMS or mobile device app Twitter Inc. is based in San Francisco and has more than 25 offices around the world.
        Twitter was created in March 2006 by Jack Dorsey, Evan Williams, Biz Stone, and Noah Glass and launched in July 2006. The service rapidly gained worldwide popularity, with more than 100 million users posting 340 million tweets a day in 2012.The service also handled 1.6 billion search queries per day.
    </div>
    <div id="facebook">
        Facebook is an online social networking service headquartered in Menlo Park, California. Its website was launched on February 4, 2004, by Mark Zuckerberg with his Harvard College roommates and fellow students Eduardo Saverin, Andrew McCollum, Dustin Moskovitz and Chris Hughes.The founders had initially limited the website's membership to Harvard students, but later expanded it to colleges in the Boston area, the Ivy League, and Stanford University. It gradually added support for students at various other universities and later to high-school students.
    </div>
    <div id="whatsapp">
        WhatsApp Messenger is a proprietary cross-platform instant messaging client for smart phones that operates under a subscription business model. It uses the Internet to send text messages, images, video, user location and audio media messages to other users using standard cellular mobile numbers.
        As of February 2016, WhatsApp had a user base of up to one billion,[10] making it the most globally popular messaging application.
        WhatsApp Inc., based in Mountain View, California, was acquired by Facebook Inc. on February 19, 2014, for approximately US$19.3 billion.
    </div>
</ej-tab>
<button type="button" (click)="OnClick()">GetItemsCount</button>

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
    OnClick(){

    $("#tab").ejTab("getItemsCount"); 

}
}


{% endhighlight %}









### hide()
{:#methods:hide}




This function hides the tab control.



#### Example

{% highlight html %}

<ej-tab id="tab" [allowKeyboardNavigation]=true>
    <ul>
        <li><a href="#twitter">Twitter</a></li>
        <li><a href="#facebook">Facebook</a></li>
        <li><a href="#whatsapp">WhatsApp</a></li>
    </ul>
    <div id="twitter">
        Twitter is an online social networking service that enables users to send and read short 140-character messages called "tweets".
        Registered users can read and post tweets, but those who are unregistered can only read them. Users access Twitter through the website interface, SMS or mobile device app Twitter Inc. is based in San Francisco and has more than 25 offices around the world.
        Twitter was created in March 2006 by Jack Dorsey, Evan Williams, Biz Stone, and Noah Glass and launched in July 2006. The service rapidly gained worldwide popularity, with more than 100 million users posting 340 million tweets a day in 2012.The service also handled 1.6 billion search queries per day.
    </div>
    <div id="facebook">
        Facebook is an online social networking service headquartered in Menlo Park, California. Its website was launched on February 4, 2004, by Mark Zuckerberg with his Harvard College roommates and fellow students Eduardo Saverin, Andrew McCollum, Dustin Moskovitz and Chris Hughes.The founders had initially limited the website's membership to Harvard students, but later expanded it to colleges in the Boston area, the Ivy League, and Stanford University. It gradually added support for students at various other universities and later to high-school students.
    </div>
    <div id="whatsapp">
        WhatsApp Messenger is a proprietary cross-platform instant messaging client for smart phones that operates under a subscription business model. It uses the Internet to send text messages, images, video, user location and audio media messages to other users using standard cellular mobile numbers.
        As of February 2016, WhatsApp had a user base of up to one billion,[10] making it the most globally popular messaging application.
        WhatsApp Inc., based in Mountain View, California, was acquired by Facebook Inc. on February 19, 2014, for approximately US$19.3 billion.
    </div>
</ej-tab>
<button type="button" (click)="OnClick()">Hide</button>

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
    OnClick(){


var obj = $("#tab").data("ejTab");


obj.hide();

}
}


{% endhighlight %}

{% highlight html %}

<ej-tab id="tab" [allowKeyboardNavigation]=true>
    <ul>
        <li><a href="#twitter">Twitter</a></li>
        <li><a href="#facebook">Facebook</a></li>
        <li><a href="#whatsapp">WhatsApp</a></li>
    </ul>
    <div id="twitter">
        Twitter is an online social networking service that enables users to send and read short 140-character messages called "tweets".
        Registered users can read and post tweets, but those who are unregistered can only read them. Users access Twitter through the website interface, SMS or mobile device app Twitter Inc. is based in San Francisco and has more than 25 offices around the world.
        Twitter was created in March 2006 by Jack Dorsey, Evan Williams, Biz Stone, and Noah Glass and launched in July 2006. The service rapidly gained worldwide popularity, with more than 100 million users posting 340 million tweets a day in 2012.The service also handled 1.6 billion search queries per day.
    </div>
    <div id="facebook">
        Facebook is an online social networking service headquartered in Menlo Park, California. Its website was launched on February 4, 2004, by Mark Zuckerberg with his Harvard College roommates and fellow students Eduardo Saverin, Andrew McCollum, Dustin Moskovitz and Chris Hughes.The founders had initially limited the website's membership to Harvard students, but later expanded it to colleges in the Boston area, the Ivy League, and Stanford University. It gradually added support for students at various other universities and later to high-school students.
    </div>
    <div id="whatsapp">
        WhatsApp Messenger is a proprietary cross-platform instant messaging client for smart phones that operates under a subscription business model. It uses the Internet to send text messages, images, video, user location and audio media messages to other users using standard cellular mobile numbers.
        As of February 2016, WhatsApp had a user base of up to one billion,[10] making it the most globally popular messaging application.
        WhatsApp Inc., based in Mountain View, California, was acquired by Facebook Inc. on February 19, 2014, for approximately US$19.3 billion.
    </div>
</ej-tab>
<button type="button" (click)="OnClick()">Hide</button>

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
    OnClick(){

    $("#tab").ejTab("hide"); 

}
}


{% endhighlight %}











### hideItem(index)
{:#methods:hideitem}




This function hides the specified item tab in tab control.


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
<td class="type"><span class="param-type">number</span></td>
<td class="description">index of tab item.</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<ej-tab id="tab" [allowKeyboardNavigation]=true>
    <ul>
        <li><a href="#twitter">Twitter</a></li>
        <li><a href="#facebook">Facebook</a></li>
        <li><a href="#whatsapp">WhatsApp</a></li>
    </ul>
    <div id="twitter">
        Twitter is an online social networking service that enables users to send and read short 140-character messages called "tweets".
        Registered users can read and post tweets, but those who are unregistered can only read them. Users access Twitter through the website interface, SMS or mobile device app Twitter Inc. is based in San Francisco and has more than 25 offices around the world.
        Twitter was created in March 2006 by Jack Dorsey, Evan Williams, Biz Stone, and Noah Glass and launched in July 2006. The service rapidly gained worldwide popularity, with more than 100 million users posting 340 million tweets a day in 2012.The service also handled 1.6 billion search queries per day.
    </div>
    <div id="facebook">
        Facebook is an online social networking service headquartered in Menlo Park, California. Its website was launched on February 4, 2004, by Mark Zuckerberg with his Harvard College roommates and fellow students Eduardo Saverin, Andrew McCollum, Dustin Moskovitz and Chris Hughes.The founders had initially limited the website's membership to Harvard students, but later expanded it to colleges in the Boston area, the Ivy League, and Stanford University. It gradually added support for students at various other universities and later to high-school students.
    </div>
    <div id="whatsapp">
        WhatsApp Messenger is a proprietary cross-platform instant messaging client for smart phones that operates under a subscription business model. It uses the Internet to send text messages, images, video, user location and audio media messages to other users using standard cellular mobile numbers.
        As of February 2016, WhatsApp had a user base of up to one billion,[10] making it the most globally popular messaging application.
        WhatsApp Inc., based in Mountain View, California, was acquired by Facebook Inc. on February 19, 2014, for approximately US$19.3 billion.
    </div>
</ej-tab>
<button type="button" (click)="OnClick()">Hide</button>

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
    OnClick(){


var obj = $("#tab").data("ejTab");


obj.hideItem(1);

}
}


{% endhighlight %}

{% highlight html %}

<ej-tab id="tab" [allowKeyboardNavigation]=true>
    <ul>
        <li><a href="#twitter">Twitter</a></li>
        <li><a href="#facebook">Facebook</a></li>
        <li><a href="#whatsapp">WhatsApp</a></li>
    </ul>
    <div id="twitter">
        Twitter is an online social networking service that enables users to send and read short 140-character messages called "tweets".
        Registered users can read and post tweets, but those who are unregistered can only read them. Users access Twitter through the website interface, SMS or mobile device app Twitter Inc. is based in San Francisco and has more than 25 offices around the world.
        Twitter was created in March 2006 by Jack Dorsey, Evan Williams, Biz Stone, and Noah Glass and launched in July 2006. The service rapidly gained worldwide popularity, with more than 100 million users posting 340 million tweets a day in 2012.The service also handled 1.6 billion search queries per day.
    </div>
    <div id="facebook">
        Facebook is an online social networking service headquartered in Menlo Park, California. Its website was launched on February 4, 2004, by Mark Zuckerberg with his Harvard College roommates and fellow students Eduardo Saverin, Andrew McCollum, Dustin Moskovitz and Chris Hughes.The founders had initially limited the website's membership to Harvard students, but later expanded it to colleges in the Boston area, the Ivy League, and Stanford University. It gradually added support for students at various other universities and later to high-school students.
    </div>
    <div id="whatsapp">
        WhatsApp Messenger is a proprietary cross-platform instant messaging client for smart phones that operates under a subscription business model. It uses the Internet to send text messages, images, video, user location and audio media messages to other users using standard cellular mobile numbers.
        As of February 2016, WhatsApp had a user base of up to one billion,[10] making it the most globally popular messaging application.
        WhatsApp Inc., based in Mountain View, California, was acquired by Facebook Inc. on February 19, 2014, for approximately US$19.3 billion.
    </div>
</ej-tab>
<button type="button" (click)="OnClick()">Hide</button>

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
    OnClick(){

    $("#tab").ejTab("hideItem",1); 

}
}


{% endhighlight %}










### removeItem(index)
{:#methods:removeitem}




Remove the given index tab item.

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
<td class="type"><span class="param-type">number</span></td>
<td class="description">index of tab item.</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<ej-tab id="tab" [allowKeyboardNavigation]=true>
    <ul>
        <li><a href="#twitter">Twitter</a></li>
        <li><a href="#facebook">Facebook</a></li>
        <li><a href="#whatsapp">WhatsApp</a></li>
    </ul>
    <div id="twitter">
        Twitter is an online social networking service that enables users to send and read short 140-character messages called "tweets".
        Registered users can read and post tweets, but those who are unregistered can only read them. Users access Twitter through the website interface, SMS or mobile device app Twitter Inc. is based in San Francisco and has more than 25 offices around the world.
        Twitter was created in March 2006 by Jack Dorsey, Evan Williams, Biz Stone, and Noah Glass and launched in July 2006. The service rapidly gained worldwide popularity, with more than 100 million users posting 340 million tweets a day in 2012.The service also handled 1.6 billion search queries per day.
    </div>
    <div id="facebook">
        Facebook is an online social networking service headquartered in Menlo Park, California. Its website was launched on February 4, 2004, by Mark Zuckerberg with his Harvard College roommates and fellow students Eduardo Saverin, Andrew McCollum, Dustin Moskovitz and Chris Hughes.The founders had initially limited the website's membership to Harvard students, but later expanded it to colleges in the Boston area, the Ivy League, and Stanford University. It gradually added support for students at various other universities and later to high-school students.
    </div>
    <div id="whatsapp">
        WhatsApp Messenger is a proprietary cross-platform instant messaging client for smart phones that operates under a subscription business model. It uses the Internet to send text messages, images, video, user location and audio media messages to other users using standard cellular mobile numbers.
        As of February 2016, WhatsApp had a user base of up to one billion,[10] making it the most globally popular messaging application.
        WhatsApp Inc., based in Mountain View, California, was acquired by Facebook Inc. on February 19, 2014, for approximately US$19.3 billion.
    </div>
</ej-tab>
<button type="button" (click)="OnClick()">RemoveItem</button>

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
    OnClick(){


var obj = $("#tab").data("ejTab");


obj.removeItem(1);

}
}


{% endhighlight %}

{% highlight html %}

<ej-tab id="tab" [allowKeyboardNavigation]=true>
    <ul>
        <li><a href="#twitter">Twitter</a></li>
        <li><a href="#facebook">Facebook</a></li>
        <li><a href="#whatsapp">WhatsApp</a></li>
    </ul>
    <div id="twitter">
        Twitter is an online social networking service that enables users to send and read short 140-character messages called "tweets".
        Registered users can read and post tweets, but those who are unregistered can only read them. Users access Twitter through the website interface, SMS or mobile device app Twitter Inc. is based in San Francisco and has more than 25 offices around the world.
        Twitter was created in March 2006 by Jack Dorsey, Evan Williams, Biz Stone, and Noah Glass and launched in July 2006. The service rapidly gained worldwide popularity, with more than 100 million users posting 340 million tweets a day in 2012.The service also handled 1.6 billion search queries per day.
    </div>
    <div id="facebook">
        Facebook is an online social networking service headquartered in Menlo Park, California. Its website was launched on February 4, 2004, by Mark Zuckerberg with his Harvard College roommates and fellow students Eduardo Saverin, Andrew McCollum, Dustin Moskovitz and Chris Hughes.The founders had initially limited the website's membership to Harvard students, but later expanded it to colleges in the Boston area, the Ivy League, and Stanford University. It gradually added support for students at various other universities and later to high-school students.
    </div>
    <div id="whatsapp">
        WhatsApp Messenger is a proprietary cross-platform instant messaging client for smart phones that operates under a subscription business model. It uses the Internet to send text messages, images, video, user location and audio media messages to other users using standard cellular mobile numbers.
        As of February 2016, WhatsApp had a user base of up to one billion,[10] making it the most globally popular messaging application.
        WhatsApp Inc., based in Mountain View, California, was acquired by Facebook Inc. on February 19, 2014, for approximately US$19.3 billion.
    </div>
</ej-tab>
<button type="button" (click)="OnClick()">RemoveItem</button>

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
    OnClick(){

    $("#tab").ejTab("removeItem",1); 

}
}


{% endhighlight %}









### show()
{:#methods:show}




This function is to show the tab control.



#### Example

{% highlight html %}

<ej-tab id="tab" [allowKeyboardNavigation]=true>
    <ul>
        <li><a href="#twitter">Twitter</a></li>
        <li><a href="#facebook">Facebook</a></li>
        <li><a href="#whatsapp">WhatsApp</a></li>
    </ul>
    <div id="twitter">
        Twitter is an online social networking service that enables users to send and read short 140-character messages called "tweets".
        Registered users can read and post tweets, but those who are unregistered can only read them. Users access Twitter through the website interface, SMS or mobile device app Twitter Inc. is based in San Francisco and has more than 25 offices around the world.
        Twitter was created in March 2006 by Jack Dorsey, Evan Williams, Biz Stone, and Noah Glass and launched in July 2006. The service rapidly gained worldwide popularity, with more than 100 million users posting 340 million tweets a day in 2012.The service also handled 1.6 billion search queries per day.
    </div>
    <div id="facebook">
        Facebook is an online social networking service headquartered in Menlo Park, California. Its website was launched on February 4, 2004, by Mark Zuckerberg with his Harvard College roommates and fellow students Eduardo Saverin, Andrew McCollum, Dustin Moskovitz and Chris Hughes.The founders had initially limited the website's membership to Harvard students, but later expanded it to colleges in the Boston area, the Ivy League, and Stanford University. It gradually added support for students at various other universities and later to high-school students.
    </div>
    <div id="whatsapp">
        WhatsApp Messenger is a proprietary cross-platform instant messaging client for smart phones that operates under a subscription business model. It uses the Internet to send text messages, images, video, user location and audio media messages to other users using standard cellular mobile numbers.
        As of February 2016, WhatsApp had a user base of up to one billion,[10] making it the most globally popular messaging application.
        WhatsApp Inc., based in Mountain View, California, was acquired by Facebook Inc. on February 19, 2014, for approximately US$19.3 billion.
    </div>
</ej-tab>
<button type="button" (click)="OnClick()">Show</button>

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
    OnClick(){


var obj = $("#tab").data("ejTab");


obj.show();

}
}


{% endhighlight %}

{% highlight html %}

<ej-tab id="tab" [allowKeyboardNavigation]=true>
    <ul>
        <li><a href="#twitter">Twitter</a></li>
        <li><a href="#facebook">Facebook</a></li>
        <li><a href="#whatsapp">WhatsApp</a></li>
    </ul>
    <div id="twitter">
        Twitter is an online social networking service that enables users to send and read short 140-character messages called "tweets".
        Registered users can read and post tweets, but those who are unregistered can only read them. Users access Twitter through the website interface, SMS or mobile device app Twitter Inc. is based in San Francisco and has more than 25 offices around the world.
        Twitter was created in March 2006 by Jack Dorsey, Evan Williams, Biz Stone, and Noah Glass and launched in July 2006. The service rapidly gained worldwide popularity, with more than 100 million users posting 340 million tweets a day in 2012.The service also handled 1.6 billion search queries per day.
    </div>
    <div id="facebook">
        Facebook is an online social networking service headquartered in Menlo Park, California. Its website was launched on February 4, 2004, by Mark Zuckerberg with his Harvard College roommates and fellow students Eduardo Saverin, Andrew McCollum, Dustin Moskovitz and Chris Hughes.The founders had initially limited the website's membership to Harvard students, but later expanded it to colleges in the Boston area, the Ivy League, and Stanford University. It gradually added support for students at various other universities and later to high-school students.
    </div>
    <div id="whatsapp">
        WhatsApp Messenger is a proprietary cross-platform instant messaging client for smart phones that operates under a subscription business model. It uses the Internet to send text messages, images, video, user location and audio media messages to other users using standard cellular mobile numbers.
        As of February 2016, WhatsApp had a user base of up to one billion,[10] making it the most globally popular messaging application.
        WhatsApp Inc., based in Mountain View, California, was acquired by Facebook Inc. on February 19, 2014, for approximately US$19.3 billion.
    </div>
</ej-tab>
<button type="button" (click)="OnClick()">Show</button>

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
    OnClick(){

    $("#tab").ejTab("show"); 

}
}


{% endhighlight %}









### showItem(index)
{:#methods:showitem}




This function helps to show the specified hidden tab item in tab control.



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
<td class="type"><span class="param-type">number</span></td>
<td class="description">index of tab item.</td>
</tr>
</tbody>
</table>




#### Example

{% highlight html %}

<ej-tab id="tab" [allowKeyboardNavigation]=true>
    <ul>
        <li><a href="#twitter">Twitter</a></li>
        <li><a href="#facebook">Facebook</a></li>
        <li><a href="#whatsapp">WhatsApp</a></li>
    </ul>
    <div id="twitter">
        Twitter is an online social networking service that enables users to send and read short 140-character messages called "tweets".
        Registered users can read and post tweets, but those who are unregistered can only read them. Users access Twitter through the website interface, SMS or mobile device app Twitter Inc. is based in San Francisco and has more than 25 offices around the world.
        Twitter was created in March 2006 by Jack Dorsey, Evan Williams, Biz Stone, and Noah Glass and launched in July 2006. The service rapidly gained worldwide popularity, with more than 100 million users posting 340 million tweets a day in 2012.The service also handled 1.6 billion search queries per day.
    </div>
    <div id="facebook">
        Facebook is an online social networking service headquartered in Menlo Park, California. Its website was launched on February 4, 2004, by Mark Zuckerberg with his Harvard College roommates and fellow students Eduardo Saverin, Andrew McCollum, Dustin Moskovitz and Chris Hughes.The founders had initially limited the website's membership to Harvard students, but later expanded it to colleges in the Boston area, the Ivy League, and Stanford University. It gradually added support for students at various other universities and later to high-school students.
    </div>
    <div id="whatsapp">
        WhatsApp Messenger is a proprietary cross-platform instant messaging client for smart phones that operates under a subscription business model. It uses the Internet to send text messages, images, video, user location and audio media messages to other users using standard cellular mobile numbers.
        As of February 2016, WhatsApp had a user base of up to one billion,[10] making it the most globally popular messaging application.
        WhatsApp Inc., based in Mountain View, California, was acquired by Facebook Inc. on February 19, 2014, for approximately US$19.3 billion.
    </div>
</ej-tab>
<button type="button" (click)="OnClick()">ShowItem</button>

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
    OnClick(){


var obj = $("#tab").data("ejTab");


obj.showItem(1);

}
}


{% endhighlight %}

{% highlight html %}

<ej-tab id="tab" [allowKeyboardNavigation]=true>
    <ul>
        <li><a href="#twitter">Twitter</a></li>
        <li><a href="#facebook">Facebook</a></li>
        <li><a href="#whatsapp">WhatsApp</a></li>
    </ul>
    <div id="twitter">
        Twitter is an online social networking service that enables users to send and read short 140-character messages called "tweets".
        Registered users can read and post tweets, but those who are unregistered can only read them. Users access Twitter through the website interface, SMS or mobile device app Twitter Inc. is based in San Francisco and has more than 25 offices around the world.
        Twitter was created in March 2006 by Jack Dorsey, Evan Williams, Biz Stone, and Noah Glass and launched in July 2006. The service rapidly gained worldwide popularity, with more than 100 million users posting 340 million tweets a day in 2012.The service also handled 1.6 billion search queries per day.
    </div>
    <div id="facebook">
        Facebook is an online social networking service headquartered in Menlo Park, California. Its website was launched on February 4, 2004, by Mark Zuckerberg with his Harvard College roommates and fellow students Eduardo Saverin, Andrew McCollum, Dustin Moskovitz and Chris Hughes.The founders had initially limited the website's membership to Harvard students, but later expanded it to colleges in the Boston area, the Ivy League, and Stanford University. It gradually added support for students at various other universities and later to high-school students.
    </div>
    <div id="whatsapp">
        WhatsApp Messenger is a proprietary cross-platform instant messaging client for smart phones that operates under a subscription business model. It uses the Internet to send text messages, images, video, user location and audio media messages to other users using standard cellular mobile numbers.
        As of February 2016, WhatsApp had a user base of up to one billion,[10] making it the most globally popular messaging application.
        WhatsApp Inc., based in Mountain View, California, was acquired by Facebook Inc. on February 19, 2014, for approximately US$19.3 billion.
    </div>
</ej-tab>
<button type="button" (click)="OnClick()">ShowItem</button>

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
    OnClick(){

    $("#tab").ejTab("showItem",1); 

}
}


{% endhighlight %}







## Events




### itemActive
{:#events:itemactive}




Triggered after a tab item activated.

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
<td class="type"><ts ref="ej.Tab.Model"/>
<span class="param-type">object</span></td>
<td class="description">returns the tab model.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
<tr>
<td class="name">
prevActiveHeader</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">returns previous active tab header.</td>
</tr>
<tr>
<td class="name">
prevActiveIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns previous active index.</td>
</tr>
<tr>
<td class="name">
activeHeader</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">returns current active tab header .</td>
</tr>
<tr>
<td class="name">
activeIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns current active index.</td>
</tr>
<tr>
<td class="name">
isInteraction</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">returns, is it triggered by interaction or not.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<ej-tab id="tab" (itemActive)="itemActive($event)">
    <ul>
        <li><a href="#twitter">Twitter</a></li>
        <li><a href="#facebook">Facebook</a></li>
        <li><a href="#whatsapp">WhatsApp</a></li>
    </ul>
    <div id="twitter">
        Twitter is an online social networking service that enables users to send and read short 140-character messages called "tweets".
        Registered users can read and post tweets, but those who are unregistered can only read them. Users access Twitter through the website interface, SMS or mobile device app Twitter Inc. is based in San Francisco and has more than 25 offices around the world.
        Twitter was created in March 2006 by Jack Dorsey, Evan Williams, Biz Stone, and Noah Glass and launched in July 2006. The service rapidly gained worldwide popularity, with more than 100 million users posting 340 million tweets a day in 2012.The service also handled 1.6 billion search queries per day.
    </div>
    <div id="facebook">
        Facebook is an online social networking service headquartered in Menlo Park, California. Its website was launched on February 4, 2004, by Mark Zuckerberg with his Harvard College roommates and fellow students Eduardo Saverin, Andrew McCollum, Dustin Moskovitz and Chris Hughes.The founders had initially limited the website's membership to Harvard students, but later expanded it to colleges in the Boston area, the Ivy League, and Stanford University. It gradually added support for students at various other universities and later to high-school students.
    </div>
    <div id="whatsapp">
        WhatsApp Messenger is a proprietary cross-platform instant messaging client for smart phones that operates under a subscription business model. It uses the Internet to send text messages, images, video, user location and audio media messages to other users using standard cellular mobile numbers.
        As of February 2016, WhatsApp had a user base of up to one billion,[10] making it the most globally popular messaging application.
        WhatsApp Inc., based in Mountain View, California, was acquired by Facebook Inc. on February 19, 2014, for approximately US$19.3 billion.
    </div>
</ej-tab>

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
    itemActive(args){

}
}

{% endhighlight %}





### ajaxBeforeLoad
{:#events:ajaxbeforeload}




Triggered before AJAX content has been loaded.

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
<td class="type"><ts ref="ej.Tab.Model"/>
<span class="param-type">object</span></td>
<td class="description">returns the tab model.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
<tr>
<td class="name">
prevActiveHeader</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">returns previous active tab header.</td>
</tr>
<tr>
<td class="name">
prevActiveIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns previous active index.</td>
</tr>
<tr>
<td class="name">
activeHeader</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">returns current active tab header .</td>
</tr>
<tr>
<td class="name">
activeIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns current active index.</td>
</tr>
<tr>
<td class="name">
URL</td>
<td class="type"><span class="param-type">string
</span></td>
<td class="description">returns the URL of AJAX request</td>
</tr>
<tr>
<td class="name">
isInteraction</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">returns, is it triggered by interaction or not.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}


<div id="dish" style="width: 650px">
<ej-tab id="dishtype">
    <ul>
        <li><a href="#pizza">Pizza Menu</a></li>
        <li><a href="#sandwich">Sandwich Menu</a></li>
    </ul>
    <div id="pizza" style="background-color: #F5F5F5">
        <p>Pizza cooked to perfection tossed with milk, vegetables, potatoes, poultry, 100% pure mutton, and cheese - and in creating nutritious and tasty meals to maintain good health.</p>
        <div id="pizza">
        <ej-tab id="pizza" [ajaxSettings.dataType]="dataType" [ajaxSettings.contentType]="contentType" [ajaxSettings.async]="async" [ajaxSettings.data]="data" [ajaxSettings.type]="type" [ajaxSettings.cache]="cache" (ajaxBeforeLoad)="ajaxBeforeLoad($event)">
            <ul>
                <li>
                    <a href="content/cornSpinach.html">Corn & Spinach </a></li>
                <li>
                    <a href="Content/chickenDelite.html">Chicken Delite </a></li>
            </ul>
        </ej-tab>
        </div>
    </div>
    <div id="sandwich" style="background-color: #F5F5F5">
        <p>Sandwich cooked to perfection tossed with bread, milk, vegetables, potatoes, poultry, 100% pure mutton, and cheese - and in creating nutritious and tasty meals to maintain good health.</p>
        <div id="sandwich">
        <ej-tab id="sandwich" [ajaxSettings.dataType]="dataType" [ajaxSettings.contentType]="contentType" [ajaxSettings.async]="async" [ajaxSettings.data]="data" [ajaxSettings.type]="type" [ajaxSettings.cache]="cache" (ajaxBeforeLoad)="ajaxBeforeLoad($event)">
            <ul>
                <li>
                    <a href="Content/gardenVeggie.html">Garden Veggie </a></li>
                <li>
                    <a href="Content/chickenTikka.html">Chicken Tikka </a></li>
                <li>
                    <a href="Content/paneerTikka.html">Paneer Tikka </a></li>
            </ul>
            </ej-tab>
        </div>
    </div>
    </ej-tab>
</div>


{% endhighlight %}


{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './tab.component.html',
    styleUrls: ['./tab.component.css'],
    encapsulation: ViewEncapsulation.None,
})
export class ScrollTabComponent {
    dataType: any;

contentType: any;

async: any;
    cache: any;
    data: Object;
    type: any;
    constructor() {
        this.cache= false;
        this.data= {};
        this.type= 'GET';
    
this.dataType= "html";


this.contentType= "html";


this.async= true;
    }
    ajaxBeforeLoad(args){

    }
} 

{% endhighlight %}

The file ‘**cornSpinach.html**’ content is as follows. 

{% highlight html %}


    <div class="e-content">
        <img src="http://js.syncfusion.com/demos/web/images/accordion/corn-and-spinach-05.png" alt="corn-spinach"/>
        <div class="ingredients">
            Rate    : $70<br />
            Ingredients : cheese, sweet corn &amp; green capsicums.
                <br />
            Description: Small pizza bases are topped with spinach and Paneer and fresh cream, a nice layer of mozzarella cheese. This is baked until the cheese is all hot and gooey.                   
        </div>
    </div>


{% endhighlight %}



The file ‘**chickenDelite.html’** content is as follows.

{% highlight html %}


    <div class="e-content">
        <img src="http://js.syncfusion.com/demos/web/images/accordion/chicken-delite.png" alt="chicken-delite"/>
        <div class="ingredients">
            Rate    : $100<br />
            Ingredients : cheese, chicken chunks, onions &amp; pineapple chunks.  
            <br />
            Description: This is a tasty, elegant chicken dish that is easy to prepare.
        </div>
    </div>


{% endhighlight %}






### ajaxError
{:#events:ajaxerror}




Triggered if error occurs in AJAX request.

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
<td class="type"><span class="param-type">object</span></td>
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
<td class="type"><ts ref="ej.Tab.Model"/><span class="param-type">object</span></td>
<td class="description">returns the tab model.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
<tr>
<td class="name">
data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns AJAX data details.</td>
</tr>
<tr>
<td class="name">
URL</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the URL of AJAX request.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}


<div id="dish" style="width: 650px">
<ej-tab id="dishtype">
    <ul>
        <li><a href="#pizza">Pizza Menu</a></li>
        <li><a href="#sandwich">Sandwich Menu</a></li>
    </ul>
    <div id="pizza" style="background-color: #F5F5F5">
        <p>Pizza cooked to perfection tossed with milk, vegetables, potatoes, poultry, 100% pure mutton, and cheese - and in creating nutritious and tasty meals to maintain good health.</p>
        <div id="pizza">
        <ej-tab id="pizza" [ajaxSettings.dataType]="dataType" [ajaxSettings.contentType]="contentType" [ajaxSettings.async]="async" [ajaxSettings.data]="data" [ajaxSettings.type]="type" [ajaxSettings.cache]="cache" (ajaxError)="ajaxError($event)">
            <ul>
                <li>
                    <a href="content/cornSpinach.html">Corn & Spinach </a></li>
                <li>
                    <a href="Content/chickenDelite.html">Chicken Delite </a></li>
            </ul>
        </ej-tab>
        </div>
    </div>
    <div id="sandwich" style="background-color: #F5F5F5">
        <p>Sandwich cooked to perfection tossed with bread, milk, vegetables, potatoes, poultry, 100% pure mutton, and cheese - and in creating nutritious and tasty meals to maintain good health.</p>
        <div id="sandwich">
        <ej-tab id="sandwich" [ajaxSettings.dataType]="dataType" [ajaxSettings.contentType]="contentType" [ajaxSettings.async]="async" [ajaxSettings.data]="data" [ajaxSettings.type]="type" [ajaxSettings.cache]="cache" (ajaxError)="ajaxError($event)">
            <ul>
                <li>
                    <a href="Content/gardenVeggie.html">Garden Veggie </a></li>
                <li>
                    <a href="Content/chickenTikka.html">Chicken Tikka </a></li>
                <li>
                    <a href="Content/paneerTikka.html">Paneer Tikka </a></li>
            </ul>
            </ej-tab>
        </div>
    </div>
    </ej-tab>
</div>


{% endhighlight %}


{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './tab.component.html',
    styleUrls: ['./tab.component.css'],
    encapsulation: ViewEncapsulation.None,
})
export class ScrollTabComponent {
    dataType: any;

contentType: any;

async: any;
    cache: any;
    data: Object;
    type: any;
    constructor() {
        this.cache= false;
        this.data= {};
        this.type= 'GET';
    
this.dataType= "html";


this.contentType= "html";


this.async= true;
    }
    ajaxError(args){}
} 

{% endhighlight %}

The file ‘**cornSpinach.html**’ content is as follows. 

{% highlight html %}


    <div class="e-content">
        <img src="http://js.syncfusion.com/demos/web/images/accordion/corn-and-spinach-05.png" alt="corn-spinach"/>
        <div class="ingredients">
            Rate    : $70<br />
            Ingredients : cheese, sweet corn &amp; green capsicums.
                <br />
            Description: Small pizza bases are topped with spinach and Paneer and fresh cream, a nice layer of mozzarella cheese. This is baked until the cheese is all hot and gooey.                   
        </div>
    </div>


{% endhighlight %}



The file ‘**chickenDelite.html’** content is as follows.

{% highlight html %}


    <div class="e-content">
        <img src="http://js.syncfusion.com/demos/web/images/accordion/chicken-delite.png" alt="chicken-delite"/>
        <div class="ingredients">
            Rate    : $100<br />
            Ingredients : cheese, chicken chunks, onions &amp; pineapple chunks.  
            <br />
            Description: This is a tasty, elegant chicken dish that is easy to prepare.
        </div>
    </div>


{% endhighlight %}






### ajaxLoad
{:#events:ajaxload}




Triggered after AJAX content load action.

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
<td class="type"><span class="param-type">object</span></td>
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
<td class="type"><ts ref="ej.Tab.Model"/><span class="param-type">object</span></td>
<td class="description">returns the tab model.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
<tr>
<td class="name">
prevActiveHeader</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">returns previous active tab header.</td>
</tr>
<tr>
<td class="name">
prevActiveIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns previous active index.</td>
</tr>
<tr>
<td class="name">
activeHeader</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">returns current active tab header .</td>
</tr>
<tr>
<td class="name">
activeIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns current active index.</td>
</tr>
<tr>
<td class="name">
URL</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the URL of AJAX request</td>
</tr>
<tr>
<td class="name">
isInteraction</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">returns, is it triggered by interaction or not.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}


<div id="dish" style="width: 650px">
<ej-tab id="dishtype">
    <ul>
        <li><a href="#pizza">Pizza Menu</a></li>
        <li><a href="#sandwich">Sandwich Menu</a></li>
    </ul>
    <div id="pizza" style="background-color: #F5F5F5">
        <p>Pizza cooked to perfection tossed with milk, vegetables, potatoes, poultry, 100% pure mutton, and cheese - and in creating nutritious and tasty meals to maintain good health.</p>
        <div id="pizza">
        <ej-tab id="pizza" [ajaxSettings.dataType]="dataType" [ajaxSettings.contentType]="contentType" [ajaxSettings.async]="async" [ajaxSettings.data]="data" [ajaxSettings.type]="type" [ajaxSettings.cache]="cache" (ajaxLoad)="ajaxLoad($event)">
            <ul>
                <li>
                    <a href="content/cornSpinach.html">Corn & Spinach </a></li>
                <li>
                    <a href="Content/chickenDelite.html">Chicken Delite </a></li>
            </ul>
        </ej-tab>
        </div>
    </div>
    <div id="sandwich" style="background-color: #F5F5F5">
        <p>Sandwich cooked to perfection tossed with bread, milk, vegetables, potatoes, poultry, 100% pure mutton, and cheese - and in creating nutritious and tasty meals to maintain good health.</p>
        <div id="sandwich">
        <ej-tab id="sandwich" [ajaxSettings.dataType]="dataType" [ajaxSettings.contentType]="contentType" [ajaxSettings.async]="async" [ajaxSettings.data]="data" [ajaxSettings.type]="type" [ajaxSettings.cache]="cache" (ajaxLoad)="ajaxLoad($event)">
            <ul>
                <li>
                    <a href="Content/gardenVeggie.html">Garden Veggie </a></li>
                <li>
                    <a href="Content/chickenTikka.html">Chicken Tikka </a></li>
                <li>
                    <a href="Content/paneerTikka.html">Paneer Tikka </a></li>
            </ul>
            </ej-tab>
        </div>
    </div>
    </ej-tab>
</div>


{% endhighlight %}


{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './tab.component.html',
    styleUrls: ['./tab.component.css'],
    encapsulation: ViewEncapsulation.None,
})
export class ScrollTabComponent {
    dataType: any;

contentType: any;

async: any;
    cache: any;
    data: Object;
    type: any;
    constructor() {
        this.cache= false;
        this.data= {};
        this.type= 'GET';
    
this.dataType= "html";


this.contentType= "html";


this.async= true;
    }
    ajaxLoad(args){
        
    }
} 

{% endhighlight %}

The file ‘**cornSpinach.html**’ content is as follows. 

{% highlight html %}


    <div class="e-content">
        <img src="http://js.syncfusion.com/demos/web/images/accordion/corn-and-spinach-05.png" alt="corn-spinach"/>
        <div class="ingredients">
            Rate    : $70<br />
            Ingredients : cheese, sweet corn &amp; green capsicums.
                <br />
            Description: Small pizza bases are topped with spinach and Paneer and fresh cream, a nice layer of mozzarella cheese. This is baked until the cheese is all hot and gooey.                   
        </div>
    </div>


{% endhighlight %}



The file ‘**chickenDelite.html’** content is as follows.

{% highlight html %}


    <div class="e-content">
        <img src="http://js.syncfusion.com/demos/web/images/accordion/chicken-delite.png" alt="chicken-delite"/>
        <div class="ingredients">
            Rate    : $100<br />
            Ingredients : cheese, chicken chunks, onions &amp; pineapple chunks.  
            <br />
            Description: This is a tasty, elegant chicken dish that is easy to prepare.
        </div>
    </div>


{% endhighlight %}






### ajaxSuccess
{:#events:ajaxsuccess}




Triggered after a tab item activated.

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
<td class="type"><ts ref="ej.Tab.Model"/><span class="param-type">object</span></td>
<td class="description">returns the tab model.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
<tr>
<td class="name">
data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">return AJAX data.</td>
</tr>
<tr>
<td class="name">
URL</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns AJAX URL</td>
</tr>
<tr>
<td class="name">
content</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns content of AJAX request.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}


<div id="dish" style="width: 650px">
<ej-tab id="dishtype">
    <ul>
        <li><a href="#pizza">Pizza Menu</a></li>
        <li><a href="#sandwich">Sandwich Menu</a></li>
    </ul>
    <div id="pizza" style="background-color: #F5F5F5">
        <p>Pizza cooked to perfection tossed with milk, vegetables, potatoes, poultry, 100% pure mutton, and cheese - and in creating nutritious and tasty meals to maintain good health.</p>
        <div id="pizza">
        <ej-tab id="pizza" [ajaxSettings.dataType]="dataType" [ajaxSettings.contentType]="contentType" [ajaxSettings.async]="async" [ajaxSettings.data]="data" [ajaxSettings.type]="type" [ajaxSettings.cache]="cache" (ajaxSuccess)="ajaxSuccess($event)">
            <ul>
                <li>
                    <a href="content/cornSpinach.html">Corn & Spinach </a></li>
                <li>
                    <a href="Content/chickenDelite.html">Chicken Delite </a></li>
            </ul>
        </ej-tab>
        </div>
    </div>
    <div id="sandwich" style="background-color: #F5F5F5">
        <p>Sandwich cooked to perfection tossed with bread, milk, vegetables, potatoes, poultry, 100% pure mutton, and cheese - and in creating nutritious and tasty meals to maintain good health.</p>
        <div id="sandwich">
        <ej-tab id="sandwich" [ajaxSettings.dataType]="dataType" [ajaxSettings.contentType]="contentType" [ajaxSettings.async]="async" [ajaxSettings.data]="data" [ajaxSettings.type]="type" [ajaxSettings.cache]="cache" (ajaxSuccess)="ajaxSuccess($event)">
            <ul>
                <li>
                    <a href="Content/gardenVeggie.html">Garden Veggie </a></li>
                <li>
                    <a href="Content/chickenTikka.html">Chicken Tikka </a></li>
                <li>
                    <a href="Content/paneerTikka.html">Paneer Tikka </a></li>
            </ul>
            </ej-tab>
        </div>
    </div>
    </ej-tab>
</div>


{% endhighlight %}


{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './tab.component.html',
    styleUrls: ['./tab.component.css'],
    encapsulation: ViewEncapsulation.None,
})
export class ScrollTabComponent {
    dataType: any;

contentType: any;

async: any;
    cache: any;
    data: Object;
    type: any;
    constructor() {
        this.cache= false;
        this.data= {};
        this.type= 'GET';
    
this.dataType= "html";


this.contentType= "html";


this.async= true;
    }
    ajaxSuccess(args){}
} 

{% endhighlight %}

The file ‘**cornSpinach.html**’ content is as follows. 

{% highlight html %}


    <div class="e-content">
        <img src="http://js.syncfusion.com/demos/web/images/accordion/corn-and-spinach-05.png" alt="corn-spinach"/>
        <div class="ingredients">
            Rate    : $70<br />
            Ingredients : cheese, sweet corn &amp; green capsicums.
                <br />
            Description: Small pizza bases are topped with spinach and Paneer and fresh cream, a nice layer of mozzarella cheese. This is baked until the cheese is all hot and gooey.                   
        </div>
    </div>


{% endhighlight %}



The file ‘**chickenDelite.html’** content is as follows.

{% highlight html %}


    <div class="e-content">
        <img src="http://js.syncfusion.com/demos/web/images/accordion/chicken-delite.png" alt="chicken-delite"/>
        <div class="ingredients">
            Rate    : $100<br />
            Ingredients : cheese, chicken chunks, onions &amp; pineapple chunks.  
            <br />
            Description: This is a tasty, elegant chicken dish that is easy to prepare.
        </div>
    </div>


{% endhighlight %}






### beforeActive
{:#events:beforeactive}




Triggered before a tab item activated.

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
<td class="type"><ts ref="ej.Tab.Model"/><span class="param-type">object</span></td>
<td class="description">returns the tab model.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
<tr>
<td class="name">
prevActiveHeader</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">returns previous active tab header.</td>
</tr>
<tr>
<td class="name">
prevActiveIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns previous active index.</td>
</tr>
<tr>
<td class="name">
activeHeader</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">returns current active tab header .</td>
</tr>
<tr>
<td class="name">
activeIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns current active index.</td>
</tr>
<tr>
<td class="name">
isInteraction</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">returns, is it triggered by interaction or not.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<ej-tab id="tab" (beforeActive)="beforeActive($event)">
    <ul>
        <li><a href="#twitter">Twitter</a></li>
        <li><a href="#facebook">Facebook</a></li>
        <li><a href="#whatsapp">WhatsApp</a></li>
    </ul>
    <div id="twitter">
        Twitter is an online social networking service that enables users to send and read short 140-character messages called "tweets".
        Registered users can read and post tweets, but those who are unregistered can only read them. Users access Twitter through the website interface, SMS or mobile device app Twitter Inc. is based in San Francisco and has more than 25 offices around the world.
        Twitter was created in March 2006 by Jack Dorsey, Evan Williams, Biz Stone, and Noah Glass and launched in July 2006. The service rapidly gained worldwide popularity, with more than 100 million users posting 340 million tweets a day in 2012.The service also handled 1.6 billion search queries per day.
    </div>
    <div id="facebook">
        Facebook is an online social networking service headquartered in Menlo Park, California. Its website was launched on February 4, 2004, by Mark Zuckerberg with his Harvard College roommates and fellow students Eduardo Saverin, Andrew McCollum, Dustin Moskovitz and Chris Hughes.The founders had initially limited the website's membership to Harvard students, but later expanded it to colleges in the Boston area, the Ivy League, and Stanford University. It gradually added support for students at various other universities and later to high-school students.
    </div>
    <div id="whatsapp">
        WhatsApp Messenger is a proprietary cross-platform instant messaging client for smart phones that operates under a subscription business model. It uses the Internet to send text messages, images, video, user location and audio media messages to other users using standard cellular mobile numbers.
        As of February 2016, WhatsApp had a user base of up to one billion,[10] making it the most globally popular messaging application.
        WhatsApp Inc., based in Mountain View, California, was acquired by Facebook Inc. on February 19, 2014, for approximately US$19.3 billion.
    </div>
</ej-tab>

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
    beforeActive(args){

}
}

{% endhighlight %}




### beforeItemRemove
{:#events:beforeitemremove}




Triggered before a tab item remove.

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
<td class="description">Event parameters from button.
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
<td class="type"><ts ref="ej.Tab.Model"/><span class="param-type">object</span></td>
<td class="description">returns the tab model.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
<tr>
<td class="name">
index</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns current tab item index</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<ej-tab id="tab" (beforeItemRemove)="beforeItemRemove($event)">
    <ul>
        <li><a href="#twitter">Twitter</a></li>
        <li><a href="#facebook">Facebook</a></li>
        <li><a href="#whatsapp">WhatsApp</a></li>
    </ul>
    <div id="twitter">
        Twitter is an online social networking service that enables users to send and read short 140-character messages called "tweets".
        Registered users can read and post tweets, but those who are unregistered can only read them. Users access Twitter through the website interface, SMS or mobile device app Twitter Inc. is based in San Francisco and has more than 25 offices around the world.
        Twitter was created in March 2006 by Jack Dorsey, Evan Williams, Biz Stone, and Noah Glass and launched in July 2006. The service rapidly gained worldwide popularity, with more than 100 million users posting 340 million tweets a day in 2012.The service also handled 1.6 billion search queries per day.
    </div>
    <div id="facebook">
        Facebook is an online social networking service headquartered in Menlo Park, California. Its website was launched on February 4, 2004, by Mark Zuckerberg with his Harvard College roommates and fellow students Eduardo Saverin, Andrew McCollum, Dustin Moskovitz and Chris Hughes.The founders had initially limited the website's membership to Harvard students, but later expanded it to colleges in the Boston area, the Ivy League, and Stanford University. It gradually added support for students at various other universities and later to high-school students.
    </div>
    <div id="whatsapp">
        WhatsApp Messenger is a proprietary cross-platform instant messaging client for smart phones that operates under a subscription business model. It uses the Internet to send text messages, images, video, user location and audio media messages to other users using standard cellular mobile numbers.
        As of February 2016, WhatsApp had a user base of up to one billion,[10] making it the most globally popular messaging application.
        WhatsApp Inc., based in Mountain View, California, was acquired by Facebook Inc. on February 19, 2014, for approximately US$19.3 billion.
    </div>
</ej-tab>

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
    beforeItemRemove(args){

}
}

{% endhighlight %}




### create
{:#events:create}




Triggered before a tab item Create.

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
<td class="description">Event parameters from button.
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
<td class="type"><ts ref="ej.Tab.Model"/><span class="param-type">object</span></td>
<td class="description">returns the tab model.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<ej-tab id="tab" (create)="create($event)">
    <ul>
        <li><a href="#twitter">Twitter</a></li>
        <li><a href="#facebook">Facebook</a></li>
        <li><a href="#whatsapp">WhatsApp</a></li>
    </ul>
    <div id="twitter">
        Twitter is an online social networking service that enables users to send and read short 140-character messages called "tweets".
        Registered users can read and post tweets, but those who are unregistered can only read them. Users access Twitter through the website interface, SMS or mobile device app Twitter Inc. is based in San Francisco and has more than 25 offices around the world.
        Twitter was created in March 2006 by Jack Dorsey, Evan Williams, Biz Stone, and Noah Glass and launched in July 2006. The service rapidly gained worldwide popularity, with more than 100 million users posting 340 million tweets a day in 2012.The service also handled 1.6 billion search queries per day.
    </div>
    <div id="facebook">
        Facebook is an online social networking service headquartered in Menlo Park, California. Its website was launched on February 4, 2004, by Mark Zuckerberg with his Harvard College roommates and fellow students Eduardo Saverin, Andrew McCollum, Dustin Moskovitz and Chris Hughes.The founders had initially limited the website's membership to Harvard students, but later expanded it to colleges in the Boston area, the Ivy League, and Stanford University. It gradually added support for students at various other universities and later to high-school students.
    </div>
    <div id="whatsapp">
        WhatsApp Messenger is a proprietary cross-platform instant messaging client for smart phones that operates under a subscription business model. It uses the Internet to send text messages, images, video, user location and audio media messages to other users using standard cellular mobile numbers.
        As of February 2016, WhatsApp had a user base of up to one billion,[10] making it the most globally popular messaging application.
        WhatsApp Inc., based in Mountain View, California, was acquired by Facebook Inc. on February 19, 2014, for approximately US$19.3 billion.
    </div>
</ej-tab>

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
    create(args){

}
}

{% endhighlight %}





### destroy
{:#events:destroy}




Triggered before a tab item destroy.

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
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Event parameters from button.
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
<td class="type"><ts ref="ej.Tab.Model"/><span class="param-type">object</span></td>
<td class="description">returns the tab model.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<ej-tab id="tab" (destroy)="destroy($event)">
    <ul>
        <li><a href="#twitter">Twitter</a></li>
        <li><a href="#facebook">Facebook</a></li>
        <li><a href="#whatsapp">WhatsApp</a></li>
    </ul>
    <div id="twitter">
        Twitter is an online social networking service that enables users to send and read short 140-character messages called "tweets".
        Registered users can read and post tweets, but those who are unregistered can only read them. Users access Twitter through the website interface, SMS or mobile device app Twitter Inc. is based in San Francisco and has more than 25 offices around the world.
        Twitter was created in March 2006 by Jack Dorsey, Evan Williams, Biz Stone, and Noah Glass and launched in July 2006. The service rapidly gained worldwide popularity, with more than 100 million users posting 340 million tweets a day in 2012.The service also handled 1.6 billion search queries per day.
    </div>
    <div id="facebook">
        Facebook is an online social networking service headquartered in Menlo Park, California. Its website was launched on February 4, 2004, by Mark Zuckerberg with his Harvard College roommates and fellow students Eduardo Saverin, Andrew McCollum, Dustin Moskovitz and Chris Hughes.The founders had initially limited the website's membership to Harvard students, but later expanded it to colleges in the Boston area, the Ivy League, and Stanford University. It gradually added support for students at various other universities and later to high-school students.
    </div>
    <div id="whatsapp">
        WhatsApp Messenger is a proprietary cross-platform instant messaging client for smart phones that operates under a subscription business model. It uses the Internet to send text messages, images, video, user location and audio media messages to other users using standard cellular mobile numbers.
        As of February 2016, WhatsApp had a user base of up to one billion,[10] making it the most globally popular messaging application.
        WhatsApp Inc., based in Mountain View, California, was acquired by Facebook Inc. on February 19, 2014, for approximately US$19.3 billion.
    </div>
</ej-tab>

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
    destroy(args){

}
}

{% endhighlight %}





### itemAdd
{:#events:itemadd}




Triggered after new tab item add

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
<td class="type"><ts ref="ej.Tab.Model"/><span class="param-type">object</span></td>
<td class="description">returns the tab model.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
<tr>
<td class="name">
tabHeader</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">returns new added tab header.</td>
</tr>
<tr>
<td class="name">
tabContent</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns new added tab content panel.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<ej-tab id="tab" (itemAdd)="itemAdd($event)">
    <ul>
        <li><a href="#twitter">Twitter</a></li>
        <li><a href="#facebook">Facebook</a></li>
        <li><a href="#whatsapp">WhatsApp</a></li>
    </ul>
    <div id="twitter">
        Twitter is an online social networking service that enables users to send and read short 140-character messages called "tweets".
        Registered users can read and post tweets, but those who are unregistered can only read them. Users access Twitter through the website interface, SMS or mobile device app Twitter Inc. is based in San Francisco and has more than 25 offices around the world.
        Twitter was created in March 2006 by Jack Dorsey, Evan Williams, Biz Stone, and Noah Glass and launched in July 2006. The service rapidly gained worldwide popularity, with more than 100 million users posting 340 million tweets a day in 2012.The service also handled 1.6 billion search queries per day.
    </div>
    <div id="facebook">
        Facebook is an online social networking service headquartered in Menlo Park, California. Its website was launched on February 4, 2004, by Mark Zuckerberg with his Harvard College roommates and fellow students Eduardo Saverin, Andrew McCollum, Dustin Moskovitz and Chris Hughes.The founders had initially limited the website's membership to Harvard students, but later expanded it to colleges in the Boston area, the Ivy League, and Stanford University. It gradually added support for students at various other universities and later to high-school students.
    </div>
    <div id="whatsapp">
        WhatsApp Messenger is a proprietary cross-platform instant messaging client for smart phones that operates under a subscription business model. It uses the Internet to send text messages, images, video, user location and audio media messages to other users using standard cellular mobile numbers.
        As of February 2016, WhatsApp had a user base of up to one billion,[10] making it the most globally popular messaging application.
        WhatsApp Inc., based in Mountain View, California, was acquired by Facebook Inc. on February 19, 2014, for approximately US$19.3 billion.
    </div>
</ej-tab>

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
    itemAdd(args){

}
}

{% endhighlight %}





### itemRemove
{:#events:itemremove}




Triggered after tab item removed.

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
<td class="type"><ts ref="ej.Tab.Model"/><span class="param-type">object</span></td>
<td class="description">returns the tab model.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
<tr>
<td class="name">
removedTab</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">returns removed tab header.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<ej-tab id="tab" (itemActive)="itemRemove($event)">
    <ul>
        <li><a href="#twitter">Twitter</a></li>
        <li><a href="#facebook">Facebook</a></li>
        <li><a href="#whatsapp">WhatsApp</a></li>
    </ul>
    <div id="twitter">
        Twitter is an online social networking service that enables users to send and read short 140-character messages called "tweets".
        Registered users can read and post tweets, but those who are unregistered can only read them. Users access Twitter through the website interface, SMS or mobile device app Twitter Inc. is based in San Francisco and has more than 25 offices around the world.
        Twitter was created in March 2006 by Jack Dorsey, Evan Williams, Biz Stone, and Noah Glass and launched in July 2006. The service rapidly gained worldwide popularity, with more than 100 million users posting 340 million tweets a day in 2012.The service also handled 1.6 billion search queries per day.
    </div>
    <div id="facebook">
        Facebook is an online social networking service headquartered in Menlo Park, California. Its website was launched on February 4, 2004, by Mark Zuckerberg with his Harvard College roommates and fellow students Eduardo Saverin, Andrew McCollum, Dustin Moskovitz and Chris Hughes.The founders had initially limited the website's membership to Harvard students, but later expanded it to colleges in the Boston area, the Ivy League, and Stanford University. It gradually added support for students at various other universities and later to high-school students.
    </div>
    <div id="whatsapp">
        WhatsApp Messenger is a proprietary cross-platform instant messaging client for smart phones that operates under a subscription business model. It uses the Internet to send text messages, images, video, user location and audio media messages to other users using standard cellular mobile numbers.
        As of February 2016, WhatsApp had a user base of up to one billion,[10] making it the most globally popular messaging application.
        WhatsApp Inc., based in Mountain View, California, was acquired by Facebook Inc. on February 19, 2014, for approximately US$19.3 billion.
    </div>
</ej-tab>

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
    itemRemove(args){

}
}

{% endhighlight %}




