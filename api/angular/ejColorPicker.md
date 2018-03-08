---
layout: post
title: Properties, Methods and Events of ColorPicker Widget
description: API reference for ColorPicker
documentation: API
platform: angular-api
keywords: ColorPicker, Essential Angular ColorPicker, ColorPicker API 
---

# ejColorPicker

The ColorPicker control provides you a rich visual interface for color selection. You can select the color from the professionally designed palettes or custom color. By clicking a point on the color, you can change the active color to the color that is located under the pointer. 

#### Syntax

{% highlight ts %}

export class AppComponent { 
        constructor(){
                
        }
 }


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
<td class="description">settings for color picker</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %}
   
<input id="colorPicker" ej-colorpicker [value]="#278787" />

{% endhighlight %}



#### Requires



* module:jQuery


* module:ej.core.js


* module:ej.colorpicker.js


* module:ej.button.js


* module:ej.splitbutton.js


* module:ej.menu.js


* module:ej.slider.js


N> jQuery.easing external dependency has been removed from version 14.3.0.49 onwards. Kindly include this jQuery.easing dependency for versions lesser than 14.3.0.49 in order to support animation effects.


## Members


### buttonText `object`
{:#members:buttontext}


The ColorPicker control allows to define the customized text to displayed in button elements. Using the property to achieve the customized culture values.


#### Default Value

* { apply: "Apply", cancel: "Cancel", swatches: "Swatches" }

#### Example


{% highlight html %}
   
<input id="colorPicker" ej-colorpicker [value]="value" [buttonText]="buttonText"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        value: string;
        buttonText:Object;
        constructor(){
                this.value ="#278787";
                this.buttonText={apply: "Set", cancel: "Close"};
        }
 }

{% endhighlight %}

### buttonText.apply `string`
{:#members:buttontext-apply}

Sets the text for the apply button.

#### Example
 
{% highlight html %}
   
<input id="colorPicker" ej-colorpicker [value]="value" [buttonText]="buttonText"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        value: string;
        buttonText:Object;
        constructor(){
                this.value ="#278787";
                this.buttonText={apply: "select"};
        }
 }

{% endhighlight %}

### buttonText.cancel `string`
{:#members:buttontext-cancel}

Sets the text for the cancel button.

#### Example


 {% highlight html %}
   
<input id="colorPicker" ej-colorpicker [value]="value" [buttonText]="buttonText"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        value: string;
        buttonText:Object;
        constructor(){
                this.value ="#278787";
                this.buttonText={cancel: "Exit" };
        }
 }

{% endhighlight %}

### buttonText.swatches `string`
{:#members:buttontext-swatches}

Sets the header text for the swatches area.

#### Example


{% highlight html %}
   
<input id="colorPicker" ej-colorpicker [value]="value" [buttonText]="buttonText"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        value: string;
        buttonText:Object;
        constructor(){
                this.value ="#278787";
                this.buttonText={swatches: "colors"};
        }
 }

{% endhighlight %}

### buttonMode `enum|string`
{:#members:buttonmode}

<ts name="ej.ButtonMode"/>

Allows to change the mode of the button. Please refer below to know available button mode

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
Split</td>
<td class="description">Displays the button in split mode </td>
</tr>
<tr>
<td class="name">
Dropdown</td>
<td class="description">Displays the button in Dropdown mode</td>
</tr>
</tbody>
</table>


#### Default Value

* ej.ButtonMode.Split


#### Example



{% highlight html %}
   
<input id="colorPicker" ej-colorpicker [value]="value" [buttonMode]="buttonMode"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        value: string;
        buttonMode:string;
        constructor(){
                this.value ="#278787";
                this.buttonMode="dropdown";
        }
 }

{% endhighlight %}


### columns `number|string`
{:#members:columns}

Specifies the number of columns to be displayed color palette model.


#### Default Value

* 10


#### Example


{% highlight html %}
   
<input id="colorPicker" ej-colorpicker [value]="value" [columns]="columns" [modelType]="modelType"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        value: string;
        modelType:string;
        columns:number;
        constructor(){
                this.value ="#278787";
                this.columns=5;
                this.modelType="palette";
        }
 }

{% endhighlight %}


### cssClass `string`
{:#members:cssclass}

This property allows you to customize its appearance using user-defined CSS and custom skin options such as colors and backgrounds.


#### Default Value

* ""


#### Example


{% highlight html %}
   
<input id="colorPicker" ej-colorpicker [value]="value" [cssClass]="cssClass"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        value: string;
        cssClass:string;
        constructor(){
                this.value ="#278787";
                this.cssClass="gradient-lime";
        }
 }

{% endhighlight %}


### custom `array`
{:#members:custom}

This property allows to define the custom colors in the palette model.Custom palettes are created by passing a comma delimited string of HEX values or an array of colors.


#### Default Value


* empty


#### Example


{% highlight html %}
   
<input id="colorPicker" ej-colorpicker [value]="value" [modelType]="modelType" [palette]="palette" [custom]="custom"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        value: string;
        cssClass:string;
        palette:string;
        custom:string[];
        constructor(){
                this.value ="#278787";
                this.modelType="palette";
                this.palette="palette";
                this.custom= ["ffffff", "ffccff", "ff99ff", "ff66ff", "ff33ff", "ff00ff", "ccffff", "ccccff"];

        }
 }

{% endhighlight %}

### displayInline `boolean`
{:#members:displayinline}

This property allows to embed the popup in the order of DOM element flow . When we set the value as true, the color picker popup is always in visible state.


#### Default Value

* false


#### Example


{% highlight html %}
   
<input id="colorPicker" ej-colorpicker [value]="value" [displayInline]="displayInline"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        value: string;
        displayInline:boolean;
        constructor(){
                this.value ="#278787";
                this.displayInline="true";
        }
 }

{% endhighlight %}

### enabled `boolean`
{:#members:enabled}

This property allows to change the control in enabled or disabled state.


#### Default Value

* true


#### Example


{% highlight html %}
   
<input id="colorPicker" ej-colorpicker [value]="value" [enabled]="enabled"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        value: string;
        enabled:boolean;
        constructor(){
                this.value ="#278787";
                this.enabled="true";
        }
 }

{% endhighlight %}

### enableOpacity `boolean`
{:#members:enableopacity}

This property allows to enable or disable the opacity slider in the color picker control


#### Default Value

* true


#### Example

{% highlight html %}
   
<input id="colorPicker" ej-colorpicker [value]="value" [enableOpacity]="enableOpacity"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        value: string;
        enableOpacity:boolean;
        constructor(){
                this.value ="#278787";
                this.enableOpacity="true";
        }
 }

{% endhighlight %}

### htmlAttributes `object`
{:#members:htmlattributes}

It allows to define the characteristics of the ColorPicker control. It will helps to extend the capability of an HTML element.


#### Default Value

* {}


#### Example

{% highlight html %}
   
<input id="colorPicker" ej-colorpicker [value]="value" [htmlAttributes]="htmlAttributes"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        value: string;
        htmlAttributes:Object;
        constructor(){
                this.value ="#278787";
                this.htmlAttributes={disabled:"disabled"};
        }
 }

{% endhighlight %}

### locale `string`
{:#members:locale}

Defines the localized text values in button and tooltip.

#### Default Value

* "en-US"

#### Example

{% highlight html %}
   
<input id="colorPicker" ej-colorpicker [value]="value" [locale]="locale"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        value: string;
        locale:string;
        constructor(){
                this.value ="#278787";
                this.locale="zh-CN";
        }
 }

      ej.ColorPicker.Locale["zh-CN"] = {
            buttonText: {
                apply: "应用",
                cancel: "取消",
                swatches: "色板"
            },
            tooltipText: {
                switcher: "切换器",
                addbutton: "添加颜色",
                basic: "基本",
                monochrome: "单色铬",
                flatcolors: "平的颜色",
                seawolf: "海狼",
                webcolors: "网颜色",
                sandy: "沙",
                pinkshades: "桃红色树荫",
                misty: "蒙蒙",
                citrus: "柑橘",
                vintage: "葡萄酒",
                moonlight: "月光",
                candycrush: "糖果粉碎",
                currentcolor: "当前颜色",
                selectedcolor: "所选颜色"
            }
        };

{% endhighlight %}

### modelType `enum|string`
{:#members:modeltype}

<ts name="ej.ColorPicker.ModelType"/>


Specifies the model type to be rendered initially in the color picker control. See below to get available ModelType


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
Palette</td>
<td class="description">support palette type mode in color picker.</td>
</tr>
<tr>
<td class="name">
Picker</td>
<td class="description">support palette type mode in color picker.</td>
</tr>
</tbody>
</table>


#### Default Value

* ej.ColorPicker.ModelType.Default

#### Example

{% highlight html %}
   
<input id="colorPicker" ej-colorpicker [value]="value" [modelType]="modelType"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        value: string;
        modelType:string;
        constructor(){
                this.value ="#278787";
                this.modelType="palette";
        }
 }

{% endhighlight %}

### opacityValue `number|string`
{:#members:opacityvalue}

This property allows to change the opacity value .The selected color opacity will be adjusted by using this opacity value.


#### Default Value

* 100


#### Example


{% highlight html %}
   
<input id="colorPicker" ej-colorpicker [value]="value" [opacityValue]="opacityValue"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        value: string;
        opacityValue:number;
        constructor(){
                this.value ="#278787";
                this.opacityValue=20;
        }
 }

{% endhighlight %}

### palette `enum|string`
{:#members:palette}


<ts name="ej.ColorPicker.Palette"/>


Specifies the palette type to be displayed at initial time in palette model.There two types of palette model available in ColorPicker control. See below available Palette

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
BasicPalette</td>
<td class="description">used to show the basic palette</td>
</tr>
<tr>
<td class="name">
CustomPalette</td>
<td class="description">used to show the custom palette</td>
</tr>
</tbody>
</table>



#### Default Value

* ej.ColorPicker.Palette.BasicPalette


#### Example


{% highlight html %}
   
<input id="colorPicker" ej-colorpicker [value]="value" [modelType]="modelType" [palette]="palette"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        value: string;
        modelType:string;
        palette:string;
        constructor(){
                this.value ="#278787";
                this.modelType="palette";
                this.palette="basicpalette";
        }
 }

{% endhighlight %}


### presetType `enum|string`
{:#members:presettype}


<ts name="ej.ColorPicker.Presets"/>


This property allows to define the preset model to be rendered initially in palette type.It consists of 12 different types of presets. Each presets have 50 colors. See below available Presets


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
Basic</td>
<td class="description">used to show the basic presets</td>
</tr>
<tr>
<td class="name">
CandyCrush</td>
<td class="description">used to show the CandyCrush colors presets</td>
</tr>
<tr>
<td class="name">
Citrus</td>
<td class="description">used to show the Citrus colors presets</td>
</tr>
<tr>
<td class="name">
FlatColors</td>
<td class="description">used to show the FlatColors presets</td>
</tr>
<tr>
<td class="name">
Misty</td>
<td class="description">used to show the Misty presets</td>
</tr>
<tr>
<td class="name">
MoonLight</td>
<td class="description">used to show the MoonLight presets</td>
</tr>
<tr>
<td class="name">
PinkShades</td>
<td class="description">used to show the PinkShades presets</td>
</tr>
<tr>
<td class="name">
Sandy</td>
<td class="description">used to show the Sandy presets</td>
</tr>
<tr>
<td class="name">
SeaWolf</td>
<td class="description">used to show the Seawolf presets</td>
</tr>
<tr>
<td class="name">
Vintage</td>
<td class="description">used to show the Vintage presets</td>
</tr>
<tr>
<td class="name">
WebColors</td>
<td class="description">used to show the WebColors presets</td>
</tr>
</tbody>
</table>

#### Default Value


* ej.ColorPicker.Presets.Basic


#### Example


{% highlight html %}
   
<input id="colorPicker" ej-colorpicker [value]="value" [modelType]="modelType" [presetType]="presetType"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        value: string;
        modelType:string;
        presetType:string;
        constructor(){
                this.value ="#278787";
                this.modelType="palette";
                this.presetType="vintage";
        }
 }

{% endhighlight %}

### showApplyCancel `boolean`
{:#members:showapplycancel}


Allows to show/hides the apply and cancel buttons in ColorPicker control


#### Default Value

* true

#### Example

{% highlight html %}
   
<input id="colorPicker" ej-colorpicker [value]="value" [showApplyCancel]="showApplyCancel"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        value: string;
        showApplyCancel:boolean;
        constructor(){
                this.value ="#278787";
                this.showApplyCancel=true;
        }
 }

{% endhighlight %}


### showClearButton `boolean`
{:#members:showclearbutton}


Allows to show/hides the clear button in ColorPicker control

#### Default Value


* true


#### Example



{% highlight html %}
   
<input id="colorPicker" ej-colorpicker [value]="value" [showClearButton]="showClearButton"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        value: string;
        showClearButton:boolean;
        constructor(){
                this.value ="#278787";
                this.showClearButton=true;
        }
 }

{% endhighlight %}

### showPreview `boolean`
{:#members:showpreview}

This property allows to provides live preview support for current cursor selection color and selected color.


#### Default Value

* true


#### Example



{% highlight html %}
   
<input id="colorPicker" ej-colorpicker [value]="value" [showPreview]="showPreview"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        value: string;
        showPreview:boolean;
        constructor(){
                this.value ="#278787";
                this.showPreview=false;
        }
 }

{% endhighlight %}

### showRecentColors `boolean`
{:#members:showrecentcolors}


This property allows to store the color values in custom list.The ColorPicker will keep up to 11 colors in a custom list.By clicking the add button, the selected color from picker or palette will get added in the recent color list.

#### Default Value

* false


#### Example


{% highlight html %}
   
<input id="colorPicker" ej-colorpicker [value]="value" [showRecentColors]="showRecentColors"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        value: string;
        showRecentColors:boolean;
        constructor(){
                this.value ="#278787";
                this.showRecentColors= true;
        }
 }

{% endhighlight %}

### showSwitcher `boolean`
{:#members:showswitcher}

Allows to show/hides the switcher button in ColorPicker control.It helps to switch palette or picker mode in color picker. 


#### Default Value

* true


#### Example

{% highlight html %}
   
<input id="colorPicker" ej-colorpicker [value]="value" [showSwitcher]="showSwitcher"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        value: string;
        showSwitcher:boolean;
        constructor(){
                this.value ="#278787";
                this.showSwitcher= false;
        }
 }

{% endhighlight %}

### showTooltip `boolean`
{:#members:showtooltip}


This property allows to shows tooltip to notify the slider value in color picker control.


#### Default Value


* false


#### Example


{% highlight html %}
   
<input id="colorPicker" ej-colorpicker [value]="value" [showTooltip]="showTooltip"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        value: string;
        showTooltip:boolean;
        constructor(){
                this.value ="#278787";
                this.showTooltip= true;
        }
 }

{% endhighlight %}



### toolIcon `string`
{:#members:toolicon}

Specifies the toolIcon to be displayed in dropdown control color area.


#### Default Value

* null


#### Example


{% highlight html %}
   
<input id="colorPicker" ej-colorpicker [value]="value" [toolIcon]="toolIcon"/>

 <style>
        .e-colorwidget .e-tool .e-fontcolor-icon:before
        {
        content: "\e632";
        margin-top: 9px;
        font-size: 10px;
        margin-left: 5px;
        }
        </style>


{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        value: string;
        toolIcon:string;
        constructor(){
                this.value ="#278787";
                this.toolIcon= "e-fontcolor-icon";
        }
 }

{% endhighlight %}


### tooltipText `object`
{:#members:tooltiptext}


This property allows to define the customized text or content to displayed when mouse over the following elements. This property also allows to use the culture values.


#### Default Value

* { switcher: "Switcher", addbutton: "Add Color", basic: "Basic", monochrome: "Mono Chrome", flatcolors: "Flat Color", seawolf: "Sea Wolf", webcolors: "Web Colors", sandy: "Sandy", pinkshades: "Pink Shades", misty: "Misty", citrus: "Citrus", vintage: "Vintage", moonlight: "Moon Light", candycrush: "Candy Crush", currentcolor: "Current Color", selectedcolor: "Selected Color" }



### tooltipText.switcher `string`
{:#members:tooltiptext-switcher}

Sets the tooltip text for the switcher button.

### tooltipText.addbutton `string`
{:#members:tooltiptext-addbutton}

Sets the tooltip text for the add button.

### tooltipText.basic `string`
{:#members:tooltiptext-basic}

Sets the tooltip text for the basic preset.

### tooltipText.monochrome `string`
{:#members:tooltiptext-monochrome}

Sets the tooltip text for the mono chrome preset.

### tooltipText.flatcolors `string`
{:#members:tooltiptext-flatcolors}

Sets the tooltip text for the flat colors preset.

### tooltipText.seawolf `string`
{:#members:tooltiptext-seawolf}

Sets the tooltip text for the sea wolf preset.

### tooltipText.webcolors `string`
{:#members:tooltiptext-webcolors}

Sets the tooltip text for the web colors preset.

### tooltipText.sandy `string`
{:#members:tooltiptext-sandy}

Sets the tooltip text for the sandy preset.

### tooltipText.pinkshades `string`
{:#members:tooltiptext-pinkshades}

Sets the tooltip text for the pink shades preset.

### tooltipText.misty `string`
{:#members:tooltiptext-misty}

Sets the tooltip text for the misty preset.

### tooltipText.citrus `string`
{:#members:tooltiptext-citrus}

Sets the tooltip text for the citrus preset.

### tooltipText.vintage `string`
{:#members:tooltiptext-vintage}

Sets the tooltip text for the vintage preset.

### tooltipText.moonlight `string`
{:#members:tooltiptext-moonlight}

Sets the tooltip text for the moon light preset.

### tooltipText.candycrush `string`
{:#members:tooltiptext-candycrush}

Sets the tooltip text for the candy crush preset.

### tooltipText.currentcolor `string`
{:#members:tooltiptext-currentcolor}

Sets the tooltip text for the current color area.

### tooltipText.selectedcolor `string`
{:#members:tooltiptext-selectedcolor}

Sets the tooltip text for the selected color area.

#### Example

{% highlight html %}
   
<input id="colorPicker" ej-colorpicker [value]="value" [tooltipText]="tooltipText"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        value: string;
        tooltipText: Object;
        constructor(){
                this.value ="#278787";
                this.tooltipText= { switcher: "Switch",  currentcolor: "New Color", selectedcolor: "Old Color" };
        }
 }

{% endhighlight %}


### value `string`
{:#members:value}

Specifies the color value for color picker control, the value is in hexadecimal form with prefix of "#".

#### Default Value

* null


#### Example


{% highlight html %}
   
<input id="colorPicker" ej-colorpicker [value]="value"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        value: string;
        tooltipText: Object;
        constructor(){
                this.value ="#278787";
        }
 }

{% endhighlight %}

## Methods


### disable()
{:#methods:disable}


Disables the color picker control


#### Example



{% highlight html %}
   
<input id="colorPicker" ej-colorpicker [value]="value"/>

{% endhighlight %}

{% highlight ts %}

 $('#colorPicker').ejColorPicker({ value: "#278787" });
        // Create ColorPicker instance
        var colorObj = $("#colorPicker").data("ejColorPicker");
        colorObj.disable(); 
        // disables the colorPicker

{% endhighlight %}


### enable()
{:#methods:enable}

Enable the color picker control


#### Example


{% highlight html %}
   
<input id="colorPicker" ej-colorpicker [value]="value"/>

{% endhighlight %}

{% highlight ts %}

 $('#colorPicker').ejColorPicker({ value: "#278787" });
        // Create ColorPicker instance
        var colorObj = $("#colorPicker").data("ejColorPicker");
        colorObj.enable(); // disables the colorPicker

{% endhighlight %}

### getColor()
{:#methods:getcolor}


Gets the selected color in RGB format

####Returns
object


#### Example



{% highlight html %}
   
<input id="colorPicker" ej-colorpicker [value]="value"/>

{% endhighlight %}

{% highlight ts %}

  $('#colorPicker').ejColorPicker({ value: "#278787" });
        // Create ColorPicker instance
        var colorObj = $("#colorPicker").data("ejColorPicker");
        var color=colorObj.getColor(); 
        // gets the selected color in RGB format
        alert("Red="+color.r+", Green="+color.g+", Blue="+color.b);

{% endhighlight %}

### getValue()
{:#methods:getvalue}

Gets the selected color value as string

####Returns

string

#### Example

{% highlight html %}
   
<input id="colorPicker" ej-colorpicker [value]="value"/>

{% endhighlight %}

{% highlight ts %}

 // Create Color picker
        $('#colorPicker').ejColorPicker({ value: "#278787" });
        // Create ColorPicker instance
        var colorObj = $("#colorPicker").data("ejColorPicker");
        alert(colorObj.getValue()); // gets the selected color value as string

{% endhighlight %}

### hexCodeToRGB(colorCode)
{:#methods:hexcodetorgb}


To Convert color value from hexCode to RGB


####Returns

object

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
colorCode </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Specified HEX code converted to RGB</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %}
   
<input id="colorPicker" ej-colorpicker [value]="value"/>

{% endhighlight %}

{% highlight ts %}

 // Create Color picker
        $('#colorPicker').ejColorPicker({ value: "#278787" });
        // Create ColorPicker instance
        var colorObj = $("#colorPicker").data("ejColorPicker");
        var color=colorObj.hexCodeToRGB("#278787"); // Convert color value from hexCode to RGB
        alert("Red="+color.r+", Green="+color.g+", Blue="+color.b);

{% endhighlight %}

### hide()
{:#methods:hide}

Hides the ColorPicker popup, if in opened state.

#### Example


{% highlight html %}
   
<input id="colorPicker" ej-colorpicker [value]="value"/>

{% endhighlight %}

{% highlight ts %}

 // Create Color picker
        $('#colorPicker').ejColorPicker({ value: "#278787" });
        // Create ColorPicker instance
        var colorObj = $("#colorPicker").data("ejColorPicker");
        colorObj.hide(); // hide the ColorPicker popup

{% endhighlight %}

### HSVToRGB(HSV)
{:#methods:hsvtorgb}

Convert color value from HSV to RGB

####Returns

object

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
HSV </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Specified HSV code converted to RGB</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %}
   
<input id="colorPicker" ej-colorpicker [value]="value"/>

{% endhighlight %}

{% highlight ts %}

 // Create Color picker
        $('#colorPicker').ejColorPicker({ value: "#278787" });
        // Create ColorPicker instance
        var colorObj = $("#colorPicker").data("ejColorPicker");
        var color=colorObj.HSVToRGB({h:230,s:98,v:98}); // Convert color value from HSV to RGB
        alert("Red="+color.r+", Green="+color.g+", Blue="+color.b);

{% endhighlight %}


### RGBToHEX(rgb)
{:#methods:rgbtohex}

Convert color value from RGB to HEX

####Returns

string

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
RGB</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Specified RGB code converted to HEX code</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}
   
<input id="colorPicker" ej-colorpicker [value]="value"/>

{% endhighlight %}

{% highlight ts %}

  // Create Color picker
        $('#colorPicker').ejColorPicker({ value: "#278787" });
        // Create ColorPicker instance
        var colorObj = $("#colorPicker").data("ejColorPicker");
        alert(colorObj.RGBToHEX(colorObj.getColor())); // Convert color value from RGB to HEX

{% endhighlight %}


### RGBToHSV(rgb)
{:#methods:rgbtohsv}

Convert color value from RGB to HSV


####Returns

object

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
RGB </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Specified RGB code converted to HSV code</td>
</tr>
</tbody>
</table>



#### Example


{% highlight html %}
   
<input id="colorPicker" ej-colorpicker [value]="value"/>

{% endhighlight %}

{% highlight ts %}

  // Create Color picker
        $('#colorPicker').ejColorPicker({ value: "#278787" });
        // Create ColorPicker instance
        var colorObj = $("#colorPicker").data("ejColorPicker");
        var color=colorObj.RGBToHSV({r:39,g:135,b:135}); // Convert color value from RGB to HSV
        alert("H="+color.r+", S="+color.g+", V="+color.b);

{% endhighlight %}


### show()
{:#methods:show}

Open the ColorPicker popup.


#### Example

{% highlight html %}
   
<input id="colorPicker" ej-colorpicker [value]="value"/>

{% endhighlight %}

{% highlight ts %}

  // Create Color picker
        $('#colorPicker').ejColorPicker({ value: "#278787" });
        // Create ColorPicker instance
        var colorObj = $("#colorPicker").data("ejColorPicker");
        colorObj.show(); // open the ColorPicker popup

{% endhighlight %}


## Events



### ejchange
{:#events:ejchange}


Fires after Color value has been changed successfully.If the user want to perform any operation after the color value changed then the user can make use of this change event.

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
<tr>
<td class="name">
changeFrom</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">return the previous color value</td>
</tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.ColorPicker.Model"/>
<span class="param-type">object</span></td>
<td class="description">returns the color picker model</td>
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
<td class="description">return the changed color value</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}
   
<input id="colorPicker" ej-colorpicker (ejchange)="onChange($event)"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onChange(e: any){ 
        // Your code here
        }

 }

{% endhighlight %}

### close
{:#events:close}


Fires after closing the color picker popup.

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
<td class="type"><ts ref="ej.ColorPicker.Model"/>
<span class="param-type">object</span></td>
<td class="description">returns the color picker model</td>
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
   
<input id="colorPicker" ej-colorpicker (close)="onClose($event)"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onClose(e: any){ 
        // Your code here
        }

 }

{% endhighlight %}


### create
{:#events:create}


Fires after Color picker control is created. If the user want to perform any operation after the color picker control creation then the user can make use of this create event.

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
<td class="name"><ts ref="ej.ColorPicker.Model"/>

model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the color picker model</td>
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
   
<input id="colorPicker" ej-colorpicker (create)="onCreate($event)"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onCreate(e: any){ 
        // Your code here
        }

 }

{% endhighlight %}

### destroy
{:#events:destroy}

Fires after Color picker control is destroyed. If the user want to perform any operation after the color picker control destroyed then the user can make use of this destroy event.

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
<td class="type"><ts ref="ej.ColorPicker.Model"/>
<span class="param-type">object</span></td>
<td class="description">returns the color picker model</td>
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
   
<input id="colorPicker" ej-colorpicker (destroy)="onDestroy($event)"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onDestroy(e: any){ 
        // Your code here
        }

 }

{% endhighlight %}

### open
{:#events:open}

Fires after opening the color picker popup

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
<td class="type"><ts ref="ej.ColorPicker.Model"/>
<span class="param-type">object</span></td>
<td class="description">returns the color picker model</td>
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
   
<input id="colorPicker" ej-colorpicker (open)="onOpen($event)"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onOpen(e: any){ 
        // Your code here
        }

 }

{% endhighlight %}

### select
{:#events:select}


Fires after Color value has been selected successfully. If the user want to perform any operation after the color value selected then the user can make use of this select event.

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
<td class="type"><ts ref="ej.ColorPicker.Model"/>
<span class="param-type">object</span></td>
<td class="description">returns the color picker model</td>
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
<td class="description">return the selected color value</td>
</tr>
</tbody>
</table>




#### Example


{% highlight html %}
   
<input id="colorPicker" ej-colorpicker (select)="onSelect($event)"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onSelect(e: any){ 
        // Your code here
        }

 }

{% endhighlight %}


