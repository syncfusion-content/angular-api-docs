---
layout: post
title: Properties, Methods and Events of ejRadioButton Widget
description: API reference for ejRadioButton
documentation: API
platform: js-api
keywords: RadioButton, ejRadioButton, syncfusion, RadioButton api 
---

# ejRadioButton



The RadioButton control allows you to choose an option to perform an action. This control allows you to select true/false.











#### Example





#### Requires



* module:jQuery

* module:ej.core.js

* module:ej.radiobutton.js


## Members




### checked `boolean`
{:#members:checked}




Specifies the check attribute of the Radio Button.


#### Default Value




* false




#### Example

CHECKED




### cssClass `string`
{:#members:cssclass}




Specify the CSS class to RadioButton to achieve custom theme.


#### Default Value




* ""




#### Example

CSSCLASS




### enabled `boolean`
{:#members:enabled}




Specifies the RadioButton control state.


#### Default Value




* true




#### Example

ENABLED




### enablePersistence `boolean`
{:#members:enablepersistence}




Specifies the enablePersistence property for RadioButton while initialization. The enablePersistence API save current model value to browser cookies for state maintains. While refreshing the radio button control page the model value apply from browser cookies.


#### Default Value




* false




#### Example

ENABLEPERSISTENCE




### enableRTL `boolean`
{:#members:enablertl}




Specify the Right to Left direction to RadioButton


#### Default Value




* false




#### Example

ENABLERTL




### htmlAttributes `object`
{:#members:htmlattributes}




Specifies the HTML Attributes of the Checkbox


#### Default Value




* {}




#### Example

HTMLATTRIBUTES




### id `string`
{:#members:id}




Specifies the id attribute for the Radio Button while initialization.


#### Default Value




* null




#### Example

ID




### idPrefix `string`
{:#members:idprefix}




Specify the idPrefix value to be added before the current id of the RadioButton.


#### Default Value




* "ej"




#### Example

IDPREFIX




### name `string`
{:#members:name}




Specifies the name attribute for the Radio Button while initialization.


#### Default Value




* Sets id as name if it is null







### size `enum`
{:#members:size}



<ts name="ej.RadioButtonSize"/>

Specifies the size of the RadioButton.


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
Small</td>
<td class="description">Shows small size radio button</td>
</tr>
<tr>
<td class="name">
Medium</td>
<td class="description">Shows medium size radio button</td>
</tr>
</tbody>
</table>




#### Default Value




* "small"




#### Example

SIZE




### text `string`
{:#members:text}




Specifies the text content for RadioButton.


#### Default Value




* ""







### validationMessage `object`
{:#members:validationmessage}




Set the jQuery validation error message in radio button.


#### Default Value




* null




#### Example

VALIDATIONMESSAGE




### validationRules `object`
{:#members:validationrules}




Set the jQuery validation rules in radio button.


#### Default Value




* null




#### Example

VALIDATIONRULES




### value `string`
{:#members:value}




Specifies the value attribute of the Radio Button.


#### Default Value




* null




#### Example

VALUE



## Methods




### disable()
{:#methods:disable}




To disable the RadioButton



#### Example

DISABLE






### enable()
{:#methods:enable}




To enable the RadioButton



#### Example

ENABLE





## Events




### beforeChange
{:#events:beforechange}




Fires before the RadioButton is going to changed its state successfully

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
<td class="type"><ts ref="ej.RadioButton.Model"/><span class="param-type">object</span></td>
<td class="description">returns the RadioButton model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
isChecked</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">returns true if element is checked, otherwise returns false</td>
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

BEFORECHANGE




### change
{:#events:change}




Fires when the RadioButton state is changed successfully

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
<td class="type"><ts ref="ej.RadioButton.Model"/><span class="param-type">object</span></td>
<td class="description">returns the RadioButton model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
isChecked</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">returns true if element is checked, otherwise returns false</td>
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

CHANGE




### create
{:#events:create}




Fires when the RadioButton created successfully

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
<td class="type"><ts ref="ej.RadioButton.Model"/><span class="param-type">object</span></td>
<td class="description">returns the RadioButton model</td>
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

CREATE




### destroy
{:#events:destroy}




Fires when the RadioButton destroyed successfully

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
<td class="type"><ts ref="ej.RadioButton.Model"/><span class="param-type">object</span></td>
<td class="description">returns the RadioButton model</td>
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

DESTROY


