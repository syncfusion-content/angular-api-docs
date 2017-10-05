---
layout: post
title: Properties,Methods and Events of Essential JS ejAutocomplete Widget
description: Methods, members, events available in ejAutocomplete
documentation: API
platform: angular-api
keywords: ejAutocomplete, API, Essential JS Autocomplete 
---

# ejAutocomplete

The AutoComplete control is a textbox control that provides a list of suggestions based on the user query.When the users enters the text in the text box, the control performs a search operation and provides a list of results in the suggestion pop up. There are several filter types available to perform the search.


#### Example


#### Requires

* module:jQuery

* module:ej.core.js

* module:ej.data.js

* module:ej.autocomplete.js

* module:ej.scroller.js

## Members

### addNewText `string`
{:#members:addnewtext}

Customize "Add New" text (label) to be added in the autocomplete popup list for the entered text when there are no suggestions for it. 

N> This property is applicable only when the “[MultiSelectMode](https://help.syncfusion.com/api/js/ejautocomplete#members:multiselectmode)” property is set as “VisualMode” and “[AllowAddNew](https://help.syncfusion.com/api/js/ejautocomplete#members:allowaddnew)” property is set as “true”.

#### Default Value:

* "Add New"

#### Example

{% highlight html %}


<input type="text" id="visualmode" ej-autocomplete width="100%" multiSelectMode="visualmode" watermarkText="Select skills" [dataSource]="language" [allowAddNew]="true" addNewText="Custom text not in list"/>

{% endhighlight %}

{% highlight ts %}


    constructor() {
        this.language = ['ActionScript', 'AppleScript', 'ASP', 'BASIC', 'BeanShell',
            'C', 'C++', 'C#', 'Clojure', 'COBOL', 'ColdFusion', 'DataFlex', 'DCL',
            'Erlang', 'E#', 'Fortran', 'F#', 'Flex', 'Google Apps Script', 'Groovy', 'Haskell', 'Hope', 'IBM HAScript',
            'Java', 'JavaScript', 'J#', 'Lisp', 'MATLAB', 'Oak', 'Perl', 'PHP',
            'Python', 'Ruby', 'Scala', 'Scheme', 'T-SQL', 'WebQL', 'ZOPL'];
    }
    
{% endhighlight %}


### allowAddNew `boolean`
{:#members:allowaddnew}

Allows new values to be added to the autocomplete input other than the values in the suggestion list. Normally, when there are no suggestions it will display “No suggestions” label in the popup.

N>  This property will work only when the “[MultiSelectMode](https://help.syncfusion.com/api/js/ejautocomplete#members:multiselectmode)” property is set as “VisualMode”

#### Default Value: 
* false

#### Example 

{% highlight html %}


<input type="text" id="visualmode" ej-autocomplete width="100%" multiSelectMode="visualmode" watermarkText="Select skills" [dataSource]="language" [allowAddNew]="true" />

{% endhighlight %}

{% highlight ts %}


    constructor() {
        this.language = ['ActionScript', 'AppleScript', 'ASP', 'BASIC', 'BeanShell',
            'C', 'C++', 'C#', 'Clojure', 'COBOL', 'ColdFusion', 'DataFlex', 'DCL',
            'Erlang', 'E#', 'Fortran', 'F#', 'Flex', 'Google Apps Script', 'Groovy', 'Haskell', 'Hope', 'IBM HAScript',
            'Java', 'JavaScript', 'J#', 'Lisp', 'MATLAB', 'Oak', 'Perl', 'PHP',
            'Python', 'Ruby', 'Scala', 'Scheme', 'T-SQL', 'WebQL', 'ZOPL'];
    }
    
{% endhighlight %}

### allowSorting `boolean`
{:#members:allowsorting}

Enables or disables the sorting of suggestion list item. The default sort order is ascending order. You customize sort order. 

{%seealso%} [SortOrder](https://help.syncfusion.com/api/js/global.html#SortOrder) {%endseealso%}

#### Default Value: 

* true

#### Example 

{% highlight html %}


<input type="text" id="visualmode" ej-autocomplete width="100%" multiSelectMode="visualmode" watermarkText="Select skills" [dataSource]="language" [allowSorting]="true"/>

{% endhighlight %}

{% highlight ts %}


    constructor() {
        this.language = ['ActionScript', 'AppleScript', 'Erlang', 'E#', 'Fortran', 'F#', 'Flex', 'Google Apps Script',
            'ASP', 'BASIC', 'BeanShell',  'COBOL', 'ColdFusion', 'DataFlex', 'DCL',
            'C', 'C++', 'C#', 'Clojure', 'Python', 'Ruby', 'Scala',
            'Groovy', 'Haskell', 'Lisp', 'MATLAB', 'Hope', 'IBM HAScript',
            'Java', 'JavaScript', 'J#', 'Oak', 'Perl', 'PHP',
             'Scheme', 'T-SQL', 'WebQL', 'ZOPL'];
    }
    
{% endhighlight %}

### animateType `enum`
{:#members:animateType}

<ts name = "ej.Autocomplete.Animation"/>

Enables or disables selecting the animation style for the popup list. Animation types can be selected through either of the following options,

<table>
<tr>
<th>Name<br/></th>
<th>Description<br/></th>
</tr>
<tr>
<td>none<br/></td>
<td>Supports to animation type with none type only.<br/></td>
</tr>
<tr>
<td>slide<br/></td>
<td>Supports to animation type with slide type only.<br/></td>
</tr>
<tr>
<td>fade<br/></td>
<td>Supports to animation type with fade type only.<br/></td>
</tr>
</table>

#### Default Value: 

* slide

#### Example 

{% highlight html %}


<input type="text" id="visualmode" ej-autocomplete width="100%" [dataSource]="language" [animateType]="animate" />

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.language = ['ActionScript', 'AppleScript', 'ASP', 'BASIC', 'BeanShell',
            'C', 'C++', 'C#', 'Clojure', 'COBOL', 'ColdFusion', 'DataFlex', 'DCL',
            'Erlang', 'E#', 'Fortran', 'F#', 'Flex', 'Google Apps Script', 'Groovy', 'Haskell', 'Hope', 'IBM HAScript',
            'Java', 'JavaScript', 'J#', 'Lisp', 'MATLAB', 'Oak', 'Perl', 'PHP',
            'Python', 'Ruby', 'Scala', 'Scheme', 'T-SQL', 'WebQL', 'ZOPL'];
        this.animate = ej.Animation.Fade;
    }
    
{% endhighlight %}

### autoFocus `boolean`
{:#members:autofocus}

To focus the items in the suggestion list when the popup is shown. By default first item will be focused. 

#### Default Value: 

* false

#### Example 

{% highlight html %}


<input type="text" id="autocompletecomp" ej-autocomplete width="100%" [dataSource]="language" [autoFocus]="true" />

{% endhighlight %}

{% highlight ts %}


    constructor() {
        this.language = ['ActionScript', 'AppleScript', 'ASP', 'BASIC', 'BeanShell',
            'C', 'C++', 'C#', 'Clojure', 'COBOL', 'ColdFusion', 'DataFlex', 'DCL',
            'Erlang', 'E#', 'Fortran', 'F#', 'Flex', 'Google Apps Script', 'Groovy', 'Haskell', 'Hope', 'IBM HAScript',
            'Java', 'JavaScript', 'J#', 'Lisp', 'MATLAB', 'Oak', 'Perl', 'PHP',
            'Python', 'Ruby', 'Scala', 'Scheme', 'T-SQL', 'WebQL', 'ZOPL'];
    }
    
{% endhighlight %}

### caseSensitiveSearch `boolean`
{:#members:casesensitivesearch}

Enables or disables the case sensitive search.

#### Default Value: 

* false

#### Example 

{% highlight html %}


<input type="text" id="autocompletecomp" ej-autocomplete width="100%" [dataSource]="language" [caseSensitiveSearch]="true" />

{% endhighlight %}

{% highlight ts %}


    constructor() {
        this.language = ['ActionScript', 'AppleScript', 'ASP', 'BASIC', 'BeanShell',
            'C', 'C++', 'C#', 'Clojure', 'COBOL', 'ColdFusion', 'DataFlex', 'DCL',
            'Erlang', 'E#', 'Fortran', 'F#', 'Flex', 'Google Apps Script', 'Groovy', 'Haskell', 'Hope', 'IBM HAScript',
            'Java', 'JavaScript', 'J#', 'Lisp', 'MATLAB', 'Oak', 'Perl', 'PHP',
            'Python', 'Ruby', 'Scala', 'Scheme', 'T-SQL', 'WebQL', 'ZOPL'];
    }
    
{% endhighlight %}

### cssClass `string`
{:#members:cssclass}

The root class for the **Autocomplete** textbox widget which helps in customizing its theme.

#### Default Value: 

* ””

#### Example 

{% highlight html %}


<input type="text" id="autocompletecomp" ej-autocomplete width="100%" [dataSource]="language" cssClass="customCSS" />

{% endhighlight %}

{% highlight ts %}


    constructor() {
        this.language = ['ActionScript', 'AppleScript', 'ASP', 'BASIC', 'BeanShell',
            'C', 'C++', 'C#', 'Clojure', 'COBOL', 'ColdFusion', 'DataFlex', 'DCL',
            'Erlang', 'E#', 'Fortran', 'F#', 'Flex', 'Google Apps Script', 'Groovy', 'Haskell', 'Hope', 'IBM HAScript',
            'Java', 'JavaScript', 'J#', 'Lisp', 'MATLAB', 'Oak', 'Perl', 'PHP',
            'Python', 'Ruby', 'Scala', 'Scheme', 'T-SQL', 'WebQL', 'ZOPL'];
    }
    
{% endhighlight %}

{% highlight css %}


.customCSS .e-autocomplete {
        background-color: azure;
        font-weight: 700;
    }
    
{% endhighlight %}

### dataSource `Object|Array`
{:#members:datasource}

The data source contains the list of data for the suggestions list. It can be a string array or JSON array or service URL that returns JSON.

#### Default Value: 

* null

#### Example 

{% highlight html %}


<input type="text" id="visualmode" ej-autocomplete width="100%" [dataSource]="language" />

{% endhighlight %}

{% highlight ts %}


    constructor() {
        this.language = ['ActionScript', 'AppleScript', 'ASP', 'BASIC', 'BeanShell',
            'C', 'C++', 'C#', 'Clojure', 'COBOL', 'ColdFusion', 'DataFlex', 'DCL',
            'Erlang', 'E#', 'Fortran', 'F#', 'Flex', 'Google Apps Script', 'Groovy', 'Haskell', 'Hope', 'IBM HAScript',
            'Java', 'JavaScript', 'J#', 'Lisp', 'MATLAB', 'Oak', 'Perl', 'PHP',
            'Python', 'Ruby', 'Scala', 'Scheme', 'T-SQL', 'WebQL', 'ZOPL'];
    }
    
{% endhighlight %}

### delaySuggestionTimeout `number`
{:#members:delaysuggestiontimeout}

The time delay (in milliseconds) after which the suggestion popup will be shown.

#### Default Value: 

* 200

#### Example 

{% highlight html %}


<input type="text" id="visualmode" ej-autocomplete [dataSource]="language" [delaySuggestionTimeout]="400" />

{% endhighlight %}

{% highlight ts %}


    constructor() {
        this.language = ['ActionScript', 'AppleScript', 'ASP', 'BASIC', 'BeanShell',
            'C', 'C++', 'C#', 'Clojure', 'COBOL', 'ColdFusion', 'DataFlex', 'DCL',
            'Erlang', 'E#', 'Fortran', 'F#', 'Flex', 'Google Apps Script', 'Groovy', 'Haskell', 'Hope', 'IBM HAScript',
            'Java', 'JavaScript', 'J#', 'Lisp', 'MATLAB', 'Oak', 'Perl', 'PHP',
            'Python', 'Ruby', 'Scala', 'Scheme', 'T-SQL', 'WebQL', 'ZOPL'];
    }
    
{% endhighlight %}

### delimiterChar `string`
{:#members:delimiterchar}

The special character which acts as a separator for the given words for multi-mode search i.e. the text after the delimiter are considered as a separate word or query for search operation. 

N> 1. This property is applicable only when the “[MultiSelectMode](https://help.syncfusion.com/api/js/ejautocomplete#members:multiselectmode)” property set as “Delimiter”.
N> 2. The delimiter string should have a single character and must be a symbol. 
N> 3. Mostly the delimiter symbol is used as (comma ,) or (semi-colon ;) or any other special character.

#### Default Value: 

* ’,’

#### Example 

{% highlight html %}


<input type="text" id="visualmode" ej-autocomplete width="100%" multiSelectMode="delimiter" [dataSource]="language" [delimiterChar]=";" />

{% endhighlight %}

{% highlight ts %}


    constructor() {
        this.language = ['ActionScript', 'AppleScript', 'ASP', 'BASIC', 'BeanShell',
            'C', 'C++', 'C#', 'Clojure', 'COBOL', 'ColdFusion', 'DataFlex', 'DCL',
            'Erlang', 'E#', 'Fortran', 'F#', 'Flex', 'Google Apps Script', 'Groovy', 'Haskell', 'Hope', 'IBM HAScript',
            'Java', 'JavaScript', 'J#', 'Lisp', 'MATLAB', 'Oak', 'Perl', 'PHP',
            'Python', 'Ruby', 'Scala', 'Scheme', 'T-SQL', 'WebQL', 'ZOPL'];
    }
    
{% endhighlight %}

### emptyResultText `string`
{:#members:emptyresulttext}

The text to be displayed in the popup when there are no suggestions available for the entered text.

N> This property is applicable only when the [showEmptyResultText](https://help.syncfusion.com/api/js/ejautocomplete#members:showemptyresulttext) property set as “true”

#### Default Value: 

* “No suggestions”

#### Example 

{% highlight html %}


<input type="text" id="visualmode" ej-autocomplete [dataSource]="language" [emptyResultText]="Suggestion not found" />

{% endhighlight %}

{% highlight ts %}


    constructor() {
        this.language = ['ActionScript', 'AppleScript', 'ASP', 'BASIC', 'BeanShell',
            'C', 'C++', 'C#', 'Clojure', 'COBOL', 'ColdFusion', 'DataFlex', 'DCL',
            'Erlang', 'E#', 'Fortran', 'F#', 'Flex', 'Google Apps Script', 'Groovy', 'Haskell', 'Hope', 'IBM HAScript',
            'Java', 'JavaScript', 'J#', 'Lisp', 'MATLAB', 'Oak', 'Perl', 'PHP',
            'Python', 'Ruby', 'Scala', 'Scheme', 'T-SQL', 'WebQL', 'ZOPL'];
    }
    
{% endhighlight %}

### enableAutoFill `boolean`
{:#members:enableautofill}

Fills the autocomplete textbox with the first matched item from the suggestion list automatically based on the entered text when enabled. 

N> This property works only when “[filterType](https://help.syncfusion.com/api/js/ejautocomplete#members:filtertype)” property is set as “startswith” 

#### Default Value: 

* false

#### Example 

{% highlight html %}


<input type="text" id="visualmode" ej-autocomplete [dataSource]="language" [enableAutoFill]="true" />

{% endhighlight %}

{% highlight ts %}


    constructor() {
        this.language = ['ActionScript', 'AppleScript', 'ASP', 'BASIC', 'BeanShell',
            'C', 'C++', 'C#', 'Clojure', 'COBOL', 'ColdFusion', 'DataFlex', 'DCL',
            'Erlang', 'E#', 'Fortran', 'F#', 'Flex', 'Google Apps Script', 'Groovy', 'Haskell', 'Hope', 'IBM HAScript',
            'Java', 'JavaScript', 'J#', 'Lisp', 'MATLAB', 'Oak', 'Perl', 'PHP',
            'Python', 'Ruby', 'Scala', 'Scheme', 'T-SQL', 'WebQL', 'ZOPL'];
    }
    
{% endhighlight %}

### enabled `boolean`
{:#members:enabled}

Enables or disables the **Autocomplete** textbox widget.

#### Default Value: 

* true

#### Example 

{% highlight html %}


<input type="text" id="visualmode" ej-autocomplete [dataSource]="language" [enabled]="false" />

{% endhighlight %}

{% highlight ts %}


    constructor() {
        this.language = ['ActionScript', 'AppleScript', 'ASP', 'BASIC', 'BeanShell',
            'C', 'C++', 'C#', 'Clojure', 'COBOL', 'ColdFusion', 'DataFlex', 'DCL',
            'Erlang', 'E#', 'Fortran', 'F#', 'Flex', 'Google Apps Script', 'Groovy', 'Haskell', 'Hope', 'IBM HAScript',
            'Java', 'JavaScript', 'J#', 'Lisp', 'MATLAB', 'Oak', 'Perl', 'PHP',
            'Python', 'Ruby', 'Scala', 'Scheme', 'T-SQL', 'WebQL', 'ZOPL'];
    }
    
{% endhighlight %}

### enableDistinct `boolean`
{:#members:enabledistinct}

Enables or disables displaying the duplicate names present in the search result.

#### Default Value: 

* false

#### Example 

{% highlight html %}


<input type="text" id="visualmode" ej-autocomplete [dataSource]="language" [enableDistinct]="true" />

{% endhighlight %}

{% highlight ts %}


    constructor() {
        this.language = ['ActionScript', 'AppleScript', 'ASP', 'BASIC', 'Java', 'BeanShell',
            'C', 'C++', 'C#', 'Clojure', 'Lisp', 'COBOL', 'ColdFusion', 'DataFlex', 'DCL',
            'Erlang', 'E#', 'Fortran', 'F#', 'Flex', 'Google Apps Script', 'Groovy', 'Haskell', 'Hope', 'IBM HAScript',
            'Java', 'JavaScript', 'J#', 'Lisp', 'MATLAB', 'ColdFusion', 'Oak', 'Perl', 'PHP',
            'Python', 'Ruby', 'Scala', 'Scheme', 'T-SQL', 'WebQL', 'ZOPL'];
    }
    
{% endhighlight %}

### enablePersistence `boolean`
{:#members:enablepersistence}

Allows the current model values to be saved in local storage or browser cookies for state maintenance when it is set to true. While refreshing the page, it retains the model value from browser cookies or local storage.

N> [Local storage](http://www.w3schools.com/html/html5_webstorage.asp#) is supported only in Html5 supported browsers. If the browsers don’t have support for local storage, browser cookies will be used to maintain the state.

#### Default Value: 

* false

#### Example 

{% highlight html %}


<input type="text" id="visualmode" ej-autocomplete [dataSource]="language" [enablePersistence]="true" />

{% endhighlight %}

{% highlight ts %}


    constructor() {
        this.language = ['ActionScript', 'AppleScript', 'ASP', 'BASIC', 'BeanShell',
            'C', 'C++', 'C#', 'Clojure', 'COBOL', 'ColdFusion', 'DataFlex', 'DCL',
            'Erlang', 'E#', 'Fortran', 'F#', 'Flex', 'Google Apps Script', 'Groovy', 'Haskell', 'Hope', 'IBM HAScript',
            'Java', 'JavaScript', 'J#', 'Lisp', 'MATLAB', 'Oak', 'Perl', 'PHP',
            'Python', 'Ruby', 'Scala', 'Scheme', 'T-SQL', 'WebQL', 'ZOPL'];
    }
    
{% endhighlight %}

### enableRTL `boolean`
{:#members:enablertl}

Displays the Autocomplete widget’s content from right to left when enabled.

#### Default Value: 

* false

#### Example 

{% highlight html %}


<input type="text" id="visualmode" ej-autocomplete [dataSource]="language" [enableRTL]="true" />

{% endhighlight %}

{% highlight ts %}


    constructor() {
        this.language = ['ActionScript', 'AppleScript', 'ASP', 'BASIC', 'BeanShell',
            'C', 'C++', 'C#', 'Clojure', 'COBOL', 'ColdFusion', 'DataFlex', 'DCL',
            'Erlang', 'E#', 'Fortran', 'F#', 'Flex', 'Google Apps Script', 'Groovy', 'Haskell', 'Hope', 'IBM HAScript',
            'Java', 'JavaScript', 'J#', 'Lisp', 'MATLAB', 'Oak', 'Perl', 'PHP',
            'Python', 'Ruby', 'Scala', 'Scheme', 'T-SQL', 'WebQL', 'ZOPL'];
    }
    
{% endhighlight %}

### fields `Object`
{:#members:fields}

Mapping fields for the suggestion items of the **Autocomplete** textbox widget.

#### Default Value:

* null

### fields.groupBy `string`
{:#members:fields-groupBy}

Used to group the suggestion list items.

### fields.htmlAttributes `Object`
{:#members:fields-htmlAttributes}

Defines the HTML attributes such as id, class, styles for the item.

### fields.key `string`
{:#members:fields-key}

Defines the specific field name which contains unique key values for the list items.

### fields.text `string`
{:#members:fields-text}

Defines the specific field name in the data source to load the suggestion list with data.

#### Example 

{% highlight html %}


<input type="text" id="searchbox" ej-autocomplete width="100%" [dataSource]="states" [fields]="fields" />

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.fields = { text: 'countryName' };
        this.states = [
            { index: 's1', countryName: 'Alabama' }, { index: 's2', countryName: 'Alaska' },
            { index: 's3', countryName: 'Arizona' }, { index: 's4', countryName: 'Arkansas' },
            { index: 's5', countryName: 'California' }, { index: 's6', countryName: 'Colorado' },
            { index: 's20', countryName: 'Maryland' }, { index: 's21', countryName: 'Massachusetts' },
            { index: 's22', countryName: 'Michigan' }, { index: 's23', countryName: 'Montana' },
            { index: 's24', countryName: 'New Mexico' }, { index: '25', countryName: 'New York' },
            { index: '26', countryName: 'North Carolina' }, { index: 's27', countryName: 'Nevada' },
            { index: 's39', countryName: 'Vermont' }, { index: 's40', countryName: 'Virginia' },
            { index: 's41', countryName: 'Washington' }, { index: 's42', countryName: 'West Virginia' },
            { index: 's43', countryName: 'Wisconsin' }, { index: 's44', countryName: 'Wyoming' }
        ];

    }
    
{% endhighlight %}


### filterType `string`
{:#members:filtertype}

Specifies the search filter type. There are several types of search filter available such as ‘startswith’, ‘contains’, ‘endswith’, ‘lessthan’, ‘lessthanorequal’, ‘greaterthan’, ‘greaterthanorequal’, ‘equal’, ‘notequal’. 

#### Default Value:  

* ej.filterType.StartsWith

#### Example  

{% highlight html %}


<input type="text" id="visualmode" ej-autocomplete [dataSource]="language" [filterType]="type" />

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.language = ['ActionScript', 'AppleScript', 'ASP', 'BASIC', 'BeanShell',
            'C', 'C++', 'C#', 'Clojure', 'COBOL', 'ColdFusion', 'DataFlex', 'DCL',
            'Erlang', 'E#', 'Fortran', 'F#', 'Flex', 'Google Apps Script', 'Groovy', 'Haskell', 'Hope', 'IBM HAScript',
            'Java', 'JavaScript', 'J#', 'Lisp', 'MATLAB', 'Oak', 'Perl', 'PHP',
            'Python', 'Ruby', 'Scala', 'Scheme', 'T-SQL', 'WebQL', 'ZOPL'];
    }
    this.type = ej.FilterOperators.contains;
    
{% endhighlight %}

### height `string|number`
{:#members:height}

The height of the Autocomplete textbox.

#### Default Value:  

* null

#### Example  

{% highlight html %}


<input type="text" id="visualmode" ej-autocomplete height="70px" [dataSource]="language" />

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.language = ['ActionScript', 'AppleScript', 'ASP', 'BASIC', 'BeanShell',
            'C', 'C++', 'C#', 'Clojure', 'COBOL', 'ColdFusion', 'DataFlex', 'DCL',
            'Erlang', 'E#', 'Fortran', 'F#', 'Flex', 'Google Apps Script', 'Groovy', 'Haskell', 'Hope', 'IBM HAScript',
            'Java', 'JavaScript', 'J#', 'Lisp', 'MATLAB', 'Oak', 'Perl', 'PHP',
            'Python', 'Ruby', 'Scala', 'Scheme', 'T-SQL', 'WebQL', 'ZOPL'];
    }
    
{% endhighlight %}

### highlightSearch `boolean`
{:#members:highlightsearch}

The search text can be highlighted in the AutoComplete suggestion list when enabled.

#### Default Value:  

* false

#### Example  

{% highlight html %}


<input type="text" id="visualmode" ej-autocomplete [dataSource]="language" [highlightSearch]="true" />

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.language = ['ActionScript', 'AppleScript', 'ASP', 'BASIC', 'BeanShell',
            'C', 'C++', 'C#', 'Clojure', 'COBOL', 'ColdFusion', 'DataFlex', 'DCL',
            'Erlang', 'E#', 'Fortran', 'F#', 'Flex', 'Google Apps Script', 'Groovy', 'Haskell', 'Hope', 'IBM HAScript',
            'Java', 'JavaScript', 'J#', 'Lisp', 'MATLAB', 'Oak', 'Perl', 'PHP',
            'Python', 'Ruby', 'Scala', 'Scheme', 'T-SQL', 'WebQL', 'ZOPL'];
    }
    
{% endhighlight %}

### itemsCount `number`
{:#members:itemscount}

Number of items to be displayed in the suggestion list.

#### Default Value:  

* 0

#### Example  

{% highlight html %}


<input type="text" id="visualmode" ej-autocomplete [dataSource]="language" [itemsCount]="count" />

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.language = ['ActionScript', 'AppleScript', 'ASP', 'BASIC', 'BeanShell',
            'C', 'C++', 'C#', 'Clojure', 'COBOL', 'ColdFusion', 'DataFlex', 'DCL',
            'Erlang', 'E#', 'Fortran', 'F#', 'Flex', 'Google Apps Script', 'Groovy', 'Haskell', 'Hope', 'IBM HAScript',
            'Java', 'JavaScript', 'J#', 'Lisp', 'MATLAB', 'Oak', 'Perl', 'PHP',
            'Python', 'Ruby', 'Scala', 'Scheme', 'T-SQL', 'WebQL', 'ZOPL'];
        this.count = 5;
    }
    
{% endhighlight %}

### locale `string`
{:#members:locale}

Set the localization culture for Autocomplete Widget.

Default Value:
{:.param}
“en-US”

Example
{:.example}


### minCharacter `number`
{:#members:mincharacter}

Minimum number of character to be entered in the Autocomplete textbox to show the suggestion list.

#### Default Value:  

* 1

#### Example  

{% highlight html %}


<input type="text" id="visualmode" ej-autocomplete [dataSource]="language" [minCharacter]="count" />

{% endhighlight %}

{% highlight ts %}


    constructor() {
        this.language = ['ActionScript', 'AppleScript', 'ASP', 'BASIC', 'BeanShell',
            'C', 'C++', 'C#', 'Clojure', 'COBOL', 'ColdFusion', 'DataFlex', 'DCL',
            'Erlang', 'E#', 'Fortran', 'F#', 'Flex', 'Google Apps Script', 'Groovy', 'Haskell', 'Hope', 'IBM HAScript',
            'Java', 'JavaScript', 'J#', 'Lisp', 'MATLAB', 'Oak', 'Perl', 'PHP',
            'Python', 'Ruby', 'Scala', 'Scheme', 'T-SQL', 'WebQL', 'ZOPL'];
        this.count = 2;
    }
    
{% endhighlight %}

### multiColumnSettings `Object`
{:#members:multicolumnsettings}

An **Autocomplete** column collection can be defined and customized through the multiColumnSettings property.
Column's header, field, and stringFormat can be define via multiColumnSettings properties.


#### Example 

{% highlight html %}


<input type="text" id="automulticolumn" ej-autocomplete [dataSource]="multicolumndataList" fields="multicolumnfields" [multiColumnSettings]="multicolumncolset" width="300px"/>

{% endhighlight %}

{% highlight ts %}

 multicolumndataList: Array<any>;
    multicolumncolset: Object;
    multicolumnfields: Object;
    value: string;
    constructor() {
        this.multicolumndataList = [{ 'EmployeeID': 1, 'FirstName': 'Nancy', 'City': 'Seattle' },
        { 'EmployeeID': 2, 'FirstName': 'Andrew', 'City': 'Tacoma' },
        { 'EmployeeID': 3, 'FirstName': 'Janet', 'City': 'Kirkland' },
        { 'EmployeeID': 4, 'FirstName': 'Margaret', 'City': 'Redmond' },
        { 'EmployeeID': 5, 'FirstName': 'Steven', 'City': 'London' },
        { 'EmployeeID': 6, 'FirstName': 'Michael', 'City': 'London' },
        { 'EmployeeID': 7, 'FirstName': 'Robert', 'City': 'London' },
        { 'EmployeeID': 8, 'FirstName': 'Laura', 'City': 'Seattle' },
        { 'EmployeeID': 9, 'FirstName': 'Anne', 'City': 'London' }]
        this.multicolumncolset = {
            stringFormat: '{0}  ({2}) ({1})',
            enable: true,
            showHeader: true,
            columns: [
                {
                    field: 'FirstName',
                    headerText: 'FirstName'
                },
                {
                    field: 'EmployeeID',
                    headerText: 'EmployeeID'
                },
                {
                    field: 'City',
                    headerText: 'City'
                }
            ]
        };
        this.multicolumnfields = { key: 'EmployeeID', text: 'FirstName' };

    }
    
{% endhighlight %}

### multiColumnSettings.enable `boolean`
{:#members:multicolumnsettings-enable}

Allow list of data to be displayed in several columns.

#### Default Value:

* false


#### Example 

{% highlight html %}


<input type="text" id="automulticolumn" ej-autocomplete [dataSource]="multicolumndataList" fields="multicolumnfields" [multiColumnSettings]="multicolumncolset" width="300px"/>

{% endhighlight %}

{% highlight ts %}

 multicolumndataList: Array<any>;
    multicolumncolset: Object;
    multicolumnfields: Object;
    value: string;
    constructor() {
        this.multicolumndataList = [{ 'EmployeeID': 1, 'FirstName': 'Nancy', 'City': 'Seattle' },
        { 'EmployeeID': 2, 'FirstName': 'Andrew', 'City': 'Tacoma' },
        { 'EmployeeID': 3, 'FirstName': 'Janet', 'City': 'Kirkland' },
        { 'EmployeeID': 4, 'FirstName': 'Margaret', 'City': 'Redmond' },
        { 'EmployeeID': 5, 'FirstName': 'Steven', 'City': 'London' },
        { 'EmployeeID': 6, 'FirstName': 'Michael', 'City': 'London' },
        { 'EmployeeID': 7, 'FirstName': 'Robert', 'City': 'London' },
        { 'EmployeeID': 8, 'FirstName': 'Laura', 'City': 'Seattle' },
        { 'EmployeeID': 9, 'FirstName': 'Anne', 'City': 'London' }]
        this.multicolumncolset = {
            stringFormat: '{0}  ({2}) ({1})',
            enable: true,
            showHeader: true,
            columns: [
                {
                    field: 'FirstName',
                    headerText: 'FirstName'
                },
                {
                    field: 'EmployeeID',
                    headerText: 'EmployeeID'
                },
                {
                    field: 'City',
                    headerText: 'City'
                }
            ]
        };
        this.multicolumnfields = { key: 'EmployeeID', text: 'FirstName' };

    }
    
{% endhighlight %}

### multiColumnSettings.showHeader `boolean`
{:#members:multicolumnsettings-showHeader}

Allow header text to be displayed in corresponding columns.

#### Default Value:

* true


#### Example 

{% highlight html %}


<input type="text" id="automulticolumn" ej-autocomplete [dataSource]="multicolumndataList" fields="multicolumnfields" [multiColumnSettings]="multicolumncolset" width="300px"/>

{% endhighlight %}

{% highlight ts %}

 multicolumndataList: Array<any>;
    multicolumncolset: Object;
    multicolumnfields: Object;
    value: string;
    constructor() {
        this.multicolumndataList = [{ 'EmployeeID': 1, 'FirstName': 'Nancy', 'City': 'Seattle' },
        { 'EmployeeID': 2, 'FirstName': 'Andrew', 'City': 'Tacoma' },
        { 'EmployeeID': 3, 'FirstName': 'Janet', 'City': 'Kirkland' },
        { 'EmployeeID': 4, 'FirstName': 'Margaret', 'City': 'Redmond' },
        { 'EmployeeID': 5, 'FirstName': 'Steven', 'City': 'London' },
        { 'EmployeeID': 6, 'FirstName': 'Michael', 'City': 'London' },
        { 'EmployeeID': 7, 'FirstName': 'Robert', 'City': 'London' },
        { 'EmployeeID': 8, 'FirstName': 'Laura', 'City': 'Seattle' },
        { 'EmployeeID': 9, 'FirstName': 'Anne', 'City': 'London' }]
        this.multicolumncolset = {
            stringFormat: '{0}  ({2}) ({1})',
            enable: true,
            showHeader: true,
            columns: [
                {
                    field: 'FirstName',
                    headerText: 'FirstName'
                },
                {
                    field: 'EmployeeID',
                    headerText: 'EmployeeID'
                },
                {
                    field: 'City',
                    headerText: 'City'
                }
            ]
        };
        this.multicolumnfields = { key: 'EmployeeID', text: 'FirstName' };

    }
    
{% endhighlight %}

### multiColumnSettings.stringFormat `string`
{:#members:multicolumnsettings-stringFormat}

Displayed selected value and autocomplete search based on mentioned column value specified in that format.

N> stringFormat as “{0} ({1}) ({2})” means search based on 0, 1 and 2 columns data.



#### Example 

{% highlight html %}


<input type="text" id="automulticolumn" ej-autocomplete [dataSource]="multicolumndataList" fields="multicolumnfields" [multiColumnSettings]="multicolumncolset" width="300px"/>

{% endhighlight %}

{% highlight ts %}

 multicolumndataList: Array<any>;
    multicolumncolset: Object;
    multicolumnfields: Object;
    value: string;
    constructor() {
        this.multicolumndataList = [{ 'EmployeeID': 1, 'FirstName': 'Nancy', 'City': 'Seattle' },
        { 'EmployeeID': 2, 'FirstName': 'Andrew', 'City': 'Tacoma' },
        { 'EmployeeID': 3, 'FirstName': 'Janet', 'City': 'Kirkland' },
        { 'EmployeeID': 4, 'FirstName': 'Margaret', 'City': 'Redmond' },
        { 'EmployeeID': 5, 'FirstName': 'Steven', 'City': 'London' },
        { 'EmployeeID': 6, 'FirstName': 'Michael', 'City': 'London' },
        { 'EmployeeID': 7, 'FirstName': 'Robert', 'City': 'London' },
        { 'EmployeeID': 8, 'FirstName': 'Laura', 'City': 'Seattle' },
        { 'EmployeeID': 9, 'FirstName': 'Anne', 'City': 'London' }]
        this.multicolumncolset = {
            stringFormat: '{0}  ({2}) ({1})',
            enable: true,
            showHeader: true,
            columns: [
                {
                    field: 'FirstName',
                    headerText: 'FirstName'
                },
                {
                    field: 'EmployeeID',
                    headerText: 'EmployeeID'
                },
                {
                    field: 'City',
                    headerText: 'City'
                }
            ]
        };
        this.multicolumnfields = { key: 'EmployeeID', text: 'FirstName' };

    }
    
{% endhighlight %}

### multiColumnSettings.columns `Array`
{:#members:multicolumnsettings-columns}

Field and Header Text collections can be defined and customized through columns field.


#### Example 

{% highlight html %}


<input type="text" id="automulticolumn" ej-autocomplete [dataSource]="multicolumndataList" fields="multicolumnfields" [multiColumnSettings]="multicolumncolset" width="300px"/>

{% endhighlight %}

{% highlight ts %}

 multicolumndataList: Array<any>;
    multicolumncolset: Object;
    multicolumnfields: Object;
    value: string;
    constructor() {
        this.multicolumndataList = [{ 'EmployeeID': 1, 'FirstName': 'Nancy', 'City': 'Seattle' },
        { 'EmployeeID': 2, 'FirstName': 'Andrew', 'City': 'Tacoma' },
        { 'EmployeeID': 3, 'FirstName': 'Janet', 'City': 'Kirkland' },
        { 'EmployeeID': 4, 'FirstName': 'Margaret', 'City': 'Redmond' },
        { 'EmployeeID': 5, 'FirstName': 'Steven', 'City': 'London' },
        { 'EmployeeID': 6, 'FirstName': 'Michael', 'City': 'London' },
        { 'EmployeeID': 7, 'FirstName': 'Robert', 'City': 'London' },
        { 'EmployeeID': 8, 'FirstName': 'Laura', 'City': 'Seattle' },
        { 'EmployeeID': 9, 'FirstName': 'Anne', 'City': 'London' }]
        this.multicolumncolset = {
            enable: true,
            columns: [
                {
                    field: 'FirstName',
                    headerText: 'FirstName'
                },
                {
                    field: 'EmployeeID',
                    headerText: 'EmployeeID'
                },
                {
                    field: 'City',
                    headerText: 'City'
                }
            ]
        };
        this.multicolumnfields = { key: 'EmployeeID', text: 'FirstName' };

    }
    
{% endhighlight %}

### multiColumnSettings.columns.field `string`
{:#members:multicolumnsettings-columns-field}

Get or set a value that indicates to display the columns in the autocomplete mapping with column name of the dataSource. 


#### Example 

{% highlight html %}


<input type="text" id="automulticolumn" ej-autocomplete [dataSource]="multicolumndataList" fields="multicolumnfields" [multiColumnSettings]="multicolumncolset" width="300px"/>

{% endhighlight %}

{% highlight ts %}

 multicolumndataList: Array<any>;
    multicolumncolset: Object;
    multicolumnfields: Object;
    value: string;
    constructor() {
        this.multicolumndataList = [{ 'EmployeeID': 1, 'FirstName': 'Nancy', 'City': 'Seattle' },
        { 'EmployeeID': 2, 'FirstName': 'Andrew', 'City': 'Tacoma' },
        { 'EmployeeID': 3, 'FirstName': 'Janet', 'City': 'Kirkland' },
        { 'EmployeeID': 4, 'FirstName': 'Margaret', 'City': 'Redmond' },
        { 'EmployeeID': 5, 'FirstName': 'Steven', 'City': 'London' },
        { 'EmployeeID': 6, 'FirstName': 'Michael', 'City': 'London' },
        { 'EmployeeID': 7, 'FirstName': 'Robert', 'City': 'London' },
        { 'EmployeeID': 8, 'FirstName': 'Laura', 'City': 'Seattle' },
        { 'EmployeeID': 9, 'FirstName': 'Anne', 'City': 'London' }]
        this.multicolumncolset = {
            stringFormat: '{0}  ({2}) ({1})',
            enable: true,
            columns: [
                {
                    field: 'FirstName'
                },
                {
                    field: 'EmployeeID'
                },
                {
                    field: 'City'
                }
            ]
        };
        this.multicolumnfields = { key: 'EmployeeID', text: 'FirstName' };

    }
    
{% endhighlight %}

### multiColumnSettings.columns.headerText `string`
{:#members:multicolumnsettings-columns-headerText}

Get or set a value that indicates to display the title of that particular column.


#### Example 

{% highlight html %}


<input type="text" id="automulticolumn" ej-autocomplete [dataSource]="multicolumndataList" fields="multicolumnfields" [multiColumnSettings]="multicolumncolset" width="300px"/>

{% endhighlight %}

{% highlight ts %}

 multicolumndataList: Array<any>;
    multicolumncolset: Object;
    multicolumnfields: Object;
    value: string;
    constructor() {
        this.multicolumndataList = [{ 'EmployeeID': 1, 'FirstName': 'Nancy', 'City': 'Seattle' },
        { 'EmployeeID': 2, 'FirstName': 'Andrew', 'City': 'Tacoma' },
        { 'EmployeeID': 3, 'FirstName': 'Janet', 'City': 'Kirkland' },
        { 'EmployeeID': 4, 'FirstName': 'Margaret', 'City': 'Redmond' },
        { 'EmployeeID': 5, 'FirstName': 'Steven', 'City': 'London' },
        { 'EmployeeID': 6, 'FirstName': 'Michael', 'City': 'London' },
        { 'EmployeeID': 7, 'FirstName': 'Robert', 'City': 'London' },
        { 'EmployeeID': 8, 'FirstName': 'Laura', 'City': 'Seattle' },
        { 'EmployeeID': 9, 'FirstName': 'Anne', 'City': 'London' }]
        this.multicolumncolset = {
            stringFormat: '{0}  ({2}) ({1})',
            enable: true,
            showHeader: true,
            columns: [
                {
                    field: 'FirstName',
                    headerText: 'FirstName'
                },
                {
                    field: 'EmployeeID',
                    headerText: 'EmployeeID'
                },
                {
                    field: 'City',
                    headerText: 'City'
                }
            ]
        };
        this.multicolumnfields = { key: 'EmployeeID', text: 'FirstName' };

    }
    
{% endhighlight %}


### multiColumnSettings.columns.cssClass `string`
{:#members:multicolumnsettings-columns-cssclass}

Gets or sets a value that indicates to render the multicolumn with custom theme. 

#### Default Value:
{:.param}
* ""

#### Example

{% highlight html %}


<input type="text" id="automulticolumn" ej-autocomplete [dataSource]="multicolumndataList" fields="multicolumnfields" [multiColumnSettings]="multicolumncolset" width="300px"/>

{% endhighlight %}

{% highlight ts %}

 multicolumndataList: Array<any>;
    multicolumncolset: Object;
    multicolumnfields: Object;
    value: string;
    constructor() {
        this.multicolumndataList = [{ 'EmployeeID': 1, 'FirstName': 'Nancy', 'City': 'Seattle' },
        { 'EmployeeID': 2, 'FirstName': 'Andrew', 'City': 'Tacoma' },
        { 'EmployeeID': 3, 'FirstName': 'Janet', 'City': 'Kirkland' },
        { 'EmployeeID': 4, 'FirstName': 'Margaret', 'City': 'Redmond' },
        { 'EmployeeID': 5, 'FirstName': 'Steven', 'City': 'London' },
        { 'EmployeeID': 6, 'FirstName': 'Michael', 'City': 'London' },
        { 'EmployeeID': 7, 'FirstName': 'Robert', 'City': 'London' },
        { 'EmployeeID': 8, 'FirstName': 'Laura', 'City': 'Seattle' },
        { 'EmployeeID': 9, 'FirstName': 'Anne', 'City': 'London' }]
        this.multicolumncolset = {
            enable: true,
            columns: [
                {
                    field: 'FirstName',
                    headerText: 'FirstName',
                    cssClass: 'importClass'
                },
                {
                    field: 'EmployeeID',
                    headerText: 'EmployeeID',
                    cssClass: 'alterClass'
                },
                {
                    field: 'City',
                    headerText: 'City',
                    cssClass: 'importClass'
                }
            ]
        };
        this.multicolumnfields = { key: 'EmployeeID', text: 'FirstName' };

    }
    
{% endhighlight %}


### multiColumnSettings.columns.type `enum`
{:#members:multicolumnsettings-columns-type}

<ts ref="ej.Type"/>

Specifies the search data type. There are four types of data types available such as string, ‘number’, ‘boolean’ and ‘date’. 

#### Default Value:  
{:.param}
* ej.Type.String

<table>
<tr>
<th>
Column type</th><th>
Data type</th></tr>
<tr>
<td>
number</td><td>
ej.Type.Number</td></tr>
<tr>
<td>
string</td><td>
ej.Type.String</td></tr>
<tr>
<td>
boolean</td><td>
ej.Type.Boolean</td></tr>
<tr>
<td>
Date</td><td>
ej.Type.Date</td></tr>
</table>


#### Example 

{% highlight html %}


<input type="text" id="automulticolumn" ej-autocomplete [dataSource]="multicolumndataList" fields="multicolumnfields" [multiColumnSettings]="multicolumncolset" width="300px"/>

{% endhighlight %}

{% highlight ts %}

 multicolumndataList: Array<any>;
    multicolumncolset: Object;
    multicolumnfields: Object;
    value: string;
    constructor() {
        this.multicolumndataList = [{ 'EmployeeID': 1, 'FirstName': 'Nancy', 'City': 'Seattle' },
        { 'EmployeeID': 2, 'FirstName': 'Andrew', 'City': 'Tacoma' },
        { 'EmployeeID': 3, 'FirstName': 'Janet', 'City': 'Kirkland' },
        { 'EmployeeID': 4, 'FirstName': 'Margaret', 'City': 'Redmond' },
        { 'EmployeeID': 5, 'FirstName': 'Steven', 'City': 'London' },
        { 'EmployeeID': 6, 'FirstName': 'Michael', 'City': 'London' },
        { 'EmployeeID': 7, 'FirstName': 'Robert', 'City': 'London' },
        { 'EmployeeID': 8, 'FirstName': 'Laura', 'City': 'Seattle' },
        { 'EmployeeID': 9, 'FirstName': 'Anne', 'City': 'London' }]
        this.multicolumncolset = {
            stringFormat: '{0}  ({2}) ({1})',
            enable: true,
            showHeader: true,
            columns: [
                {
                    field: 'FirstName',
                    headerText: 'FirstName'
                },
                {
                    field: 'EmployeeID',
                    headerText: 'EmployeeID',
                    type: ej.Type.Number
                },
                {
                    field: 'City',
                    headerText: 'City'
                }
            ]
        };
        this.multicolumnfields = { key: 'EmployeeID', text: 'FirstName' };

    }
    
{% endhighlight %}

### multiColumnSettings.columns.filterType `enum`
{:#members:multicolumnsettings-columns-filtertype}

<ts ref="ej.filterType"/>

Specifies the search filter type. There are several types of search filter available such as ‘startswith’, ‘contains’, ‘endswith’, ‘lessthan’, ‘lessthanorequal’, ‘greaterthan’, ‘greaterthanorequal’, ‘equal’, ‘notequal’. 

#### Default Value:  
{:.param}
* ej.filterType.StartsWith

<table>
<tr>
<th>
Column type</th><th>
Filter type</th></tr>
<tr>
<td>
number</td><td>
ej.filterType.GreaterThan<br/>ej.filterType.GreaterThanOrEqual<br/>ej.filterType.LessThan<br/>ej.filterType.LessThanOrEqual<br/>ej.filterType.Equal</td></tr>
<tr>
<td>
string</td><td>
ej.filterType.StartsWith<br/>ej.filterType.EndsWith<br/>ej.filterType.Contains<br/>ej.filterType.Equal<br/>ej.filterType.NotEqual</td></tr>
<tr>
<td>
boolean</td><td>
ej.filterType.Equal<br/>ej.filterType.NotEqual</td></tr>
<tr>
<td>
Date</td><td>
ej.filterType.GreaterThan<br/>ej.filterType.GreaterThanOrEqual<br/>ej.filterType.LessThan<br/>ej.filterType.LessThanOrEqual<br/>ej.filterType.Equal</td></tr>
</table>


#### Example 

{% highlight html %}


<input type="text" id="automulticolumn" ej-autocomplete [dataSource]="multicolumndataList" fields="multicolumnfields" [multiColumnSettings]="multicolumncolset" width="300px"/>

{% endhighlight %}

{% highlight ts %}

 multicolumndataList: Array<any>;
    multicolumncolset: Object;
    multicolumnfields: Object;
    value: string;
    constructor() {
        this.multicolumndataList = [{ 'EmployeeID': 1, 'FirstName': 'Nancy', 'City': 'Seattle' },
        { 'EmployeeID': 2, 'FirstName': 'Andrew', 'City': 'Tacoma' },
        { 'EmployeeID': 3, 'FirstName': 'Janet', 'City': 'Kirkland' },
        { 'EmployeeID': 4, 'FirstName': 'Margaret', 'City': 'Redmond' },
        { 'EmployeeID': 5, 'FirstName': 'Steven', 'City': 'London' },
        { 'EmployeeID': 6, 'FirstName': 'Michael', 'City': 'London' },
        { 'EmployeeID': 7, 'FirstName': 'Robert', 'City': 'London' },
        { 'EmployeeID': 8, 'FirstName': 'Laura', 'City': 'Seattle' },
        { 'EmployeeID': 9, 'FirstName': 'Anne', 'City': 'London' }]
        this.multicolumncolset = {
            stringFormat: '{0}  ({2}) ({1})',
            enable: true,
            showHeader: true,
            columns: [
                {
                    field: 'FirstName',
                    headerText: 'FirstName'
                },
                {
                    field: 'EmployeeID',
                    headerText: 'EmployeeID',
                    type: ej.Type.Number,
                    filterType: ej.filterType.GreaterThan
                },
                {
                    field: 'City',
                    headerText: 'City',
                    type: ej.Type.String,
                    filterType: ej.filterType.Contains
                }
            ]
        };
        this.multicolumnfields = { key: 'EmployeeID', text: 'FirstName' };

    }
    
{% endhighlight %}



### multiColumnSettings.columns.headerTextAlign `enum`
{:#members:multicolumnsettings-columns-headertextalign}

<ts ref="ej.TextAlign"/>

This defines the text alignment of a particular column header cell value. See headerTextAlign

#### Default Value:
{:.param}
* ej.TextAlign.Left

<table>
Add a comment to this line
<tr>
<th>Name</th>
<th>Description</th>
</tr>
<tr>
<td class="name">Center</td>
<td class="description">Header text is centered.</td>
</tr>
<tr>
<td class="name">Justify</td>
<td class="description">Header text is justified.</td>
</tr> 
<tr>
<td class="name">Left</td>
<td class="description">Header text is aligned to the left.</td>
</tr> 
<tr>
<td class="name">Right</td>
<td class="description">Header text is aligned to the right.</td>
</tr>   
</table>


#### Example 

{% highlight html %}


<input type="text" id="automulticolumn" ej-autocomplete [dataSource]="multicolumndataList" fields="multicolumnfields" [multiColumnSettings]="multicolumncolset" width="300px"/>

{% endhighlight %}

{% highlight ts %}

 multicolumndataList: Array<any>;
    multicolumncolset: Object;
    multicolumnfields: Object;
    value: string;
    constructor() {
        this.multicolumndataList = [{ 'EmployeeID': 1, 'FirstName': 'Nancy', 'City': 'Seattle' },
        { 'EmployeeID': 2, 'FirstName': 'Andrew', 'City': 'Tacoma' },
        { 'EmployeeID': 3, 'FirstName': 'Janet', 'City': 'Kirkland' },
        { 'EmployeeID': 4, 'FirstName': 'Margaret', 'City': 'Redmond' },
        { 'EmployeeID': 5, 'FirstName': 'Steven', 'City': 'London' },
        { 'EmployeeID': 6, 'FirstName': 'Michael', 'City': 'London' },
        { 'EmployeeID': 7, 'FirstName': 'Robert', 'City': 'London' },
        { 'EmployeeID': 8, 'FirstName': 'Laura', 'City': 'Seattle' },
        { 'EmployeeID': 9, 'FirstName': 'Anne', 'City': 'London' }]
        this.multicolumncolset = {
            stringFormat: '{0}  ({2}) ({1})',
            enable: true,
            showHeader: true,
            columns: [
                {
                    field: 'FirstName',
                    headerText: 'FirstName',
                    headerTextAlign: ej.TextAlign.Center
                },
                {
                    field: 'EmployeeID',
                    headerText: 'EmployeeID',
                    headerTextAlign: ej.TextAlign.Center
                },
                {
                    field: 'City',
                    headerText: 'City',
                    headerTextAlign: ej.TextAlign.Center
                }
            ]
        };
        this.multicolumnfields = { key: 'EmployeeID', text: 'FirstName' };

    }
    
{% endhighlight %}

### multiColumnSettings.columns.textAlign `enum`
{:#members:multicolumnsettings-columns-textalign}

<ts ref="ej.TextAlign"/>

Gets or sets a value that indicates to align the text within the column. See textAlign

#### Default Value:
{:.param}
* ej.TextAlign.Left

<table>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
<tr>
<td class="name">Center</td>
<td class="description">Text is centered.</td>
</tr>
<tr>
<td class="name">Justify</td>
<td class="description">Text is justified.</td>
</tr> 
<tr>
<td class="name">Left</td>
<td class="description">Text is aligned to the left.</td>
</tr> 
<tr>
<td class="name">Right</td>
<td class="description">Text is aligned to the right.</td>
</tr>   
</table>


#### Example 

{% highlight html %}


<input type="text" id="automulticolumn" ej-autocomplete [dataSource]="multicolumndataList" fields="multicolumnfields" [multiColumnSettings]="multicolumncolset" width="300px"/>

{% endhighlight %}

{% highlight ts %}

 multicolumndataList: Array<any>;
    multicolumncolset: Object;
    multicolumnfields: Object;
    value: string;
    constructor() {
        this.multicolumndataList = [{ 'EmployeeID': 1, 'FirstName': 'Nancy', 'City': 'Seattle' },
        { 'EmployeeID': 2, 'FirstName': 'Andrew', 'City': 'Tacoma' },
        { 'EmployeeID': 3, 'FirstName': 'Janet', 'City': 'Kirkland' },
        { 'EmployeeID': 4, 'FirstName': 'Margaret', 'City': 'Redmond' },
        { 'EmployeeID': 5, 'FirstName': 'Steven', 'City': 'London' },
        { 'EmployeeID': 6, 'FirstName': 'Michael', 'City': 'London' },
        { 'EmployeeID': 7, 'FirstName': 'Robert', 'City': 'London' },
        { 'EmployeeID': 8, 'FirstName': 'Laura', 'City': 'Seattle' },
        { 'EmployeeID': 9, 'FirstName': 'Anne', 'City': 'London' }]
        this.multicolumncolset = {
            stringFormat: '{0}  ({2}) ({1})',
            enable: true,
            showHeader: true,
            columns: [
                {
                    field: 'FirstName',
                    textAlign: ej.TextAlign.Right
                },
                {
                    field: 'EmployeeID',
                    textAlign: ej.TextAlign.Right
                },
                {
                    field: 'City',
                    textAlign: ej.TextAlign.Right
                }
            ]
        };
        this.multicolumnfields = { key: 'EmployeeID', text: 'FirstName' };

    }
    
{% endhighlight %}


### multiSelectMode `enum`
{:#members:multiselectmode}

<ts name = "ej.Autocomplete.MultiSelectMode"/>

Enables or disables selecting multiple values from the suggestion list. Multiple values can be selected through either of the following options,

<table>
<tr>
<th>Name<br/></th>
<th>Description<br/></th>
</tr>
<tr>
<td>Delimiter<br/></td>
<td>Multiple values are separated using a given special character.<br/></td>
</tr>
<tr>
<td>VisualMode<br/></td>
<td>Each values are displayed in separate box with close button.<br/></td>
</tr>
</table>


{%seealso%} [MultiSelectMode](https://help.syncfusion.com/api/js/global.html#MultiSelectMode) {%endseealso%}

#### Default Value:  

* ej.MultiSelectMode.None

#### Example  

{% highlight html %}


<input type="text" id="visualmode" ej-autocomplete width="100%" [multiSelectMode]="mode" watermarkText="Select skills" />

{% endhighlight %}

{% highlight ts %}


    constructor() {
        this.language = ['ActionScript', 'AppleScript', 'ASP', 'BASIC', 'BeanShell',
            'C', 'C++', 'C#', 'Clojure', 'COBOL', 'ColdFusion', 'DataFlex', 'DCL',
            'Erlang', 'E#', 'Fortran', 'F#', 'Flex', 'Google Apps Script', 'Groovy', 'Haskell', 'Hope', 'IBM HAScript',
            'Java', 'JavaScript', 'J#', 'Lisp', 'MATLAB', 'Oak', 'Perl', 'PHP',
            'Python', 'Ruby', 'Scala', 'Scheme', 'T-SQL', 'WebQL', 'ZOPL'];
        this.mode = ej.MultiSelectMode.VisualMode;
    }
    
{% endhighlight %}

### popupHeight `string`
{:#members:popupheight}

The height of the suggestion list.

#### Default Value:  

* “152px”

#### Example  

{% highlight html %}


<input type="text" id="visualmode" ej-autocomplete popupHeight="100px" [dataSource]="language" />

{% endhighlight %}

{% highlight ts %}


    constructor() {
        this.language = ['ActionScript', 'AppleScript', 'ASP', 'BASIC', 'BeanShell',
            'C', 'C++', 'C#', 'Clojure', 'COBOL', 'ColdFusion', 'DataFlex', 'DCL',
            'Erlang', 'E#', 'Fortran', 'F#', 'Flex', 'Google Apps Script', 'Groovy', 'Haskell', 'Hope', 'IBM HAScript',
            'Java', 'JavaScript', 'J#', 'Lisp', 'MATLAB', 'Oak', 'Perl', 'PHP',
            'Python', 'Ruby', 'Scala', 'Scheme', 'T-SQL', 'WebQL', 'ZOPL'];
    }
    
{% endhighlight %}

### popupWidth `string`
{:#members:popupwidth}

The width of the suggestion list.

#### Default Value:  

* “auto”

#### Example  

{% highlight html %}


<input type="text" id="visualmode" ej-autocomplete popupHeight="200px" [dataSource]="language" />

{% endhighlight %}

{% highlight ts %}


    constructor() {
        this.language = ['ActionScript', 'AppleScript', 'ASP', 'BASIC', 'BeanShell',
            'C', 'C++', 'C#', 'Clojure', 'COBOL', 'ColdFusion', 'DataFlex', 'DCL',
            'Erlang', 'E#', 'Fortran', 'F#', 'Flex', 'Google Apps Script', 'Groovy', 'Haskell', 'Hope', 'IBM HAScript',
            'Java', 'JavaScript', 'J#', 'Lisp', 'MATLAB', 'Oak', 'Perl', 'PHP',
            'Python', 'Ruby', 'Scala', 'Scheme', 'T-SQL', 'WebQL', 'ZOPL'];
    }
    
{% endhighlight %}

### query `ej.Query`
{:#members:query}

The query to retrieve the data from the data source.

#### Default Value:   

* null

#### Example  

{% highlight html %}


<input id="databindingremote" type="text" ej-autocomplete width="100%" [query]="query" [fields]="fields" watermarkText="Search a customer" [dataSource]="dataManger" />

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.fields = { text: 'ContactName', key: 'SupplierID' };
        this.dataManger = ej.DataManager({ url: 'http://js.syncfusion.com/ejServices/wcf/NorthWind.svc/', crossDomain: true }); // eslint-disable-line new-cap
        this.query = ej.Query().from('Suppliers').select('SupplierID', 'ContactName');
    }
    
{% endhighlight %}

### readOnly `boolean`
{:#members:readonly}

Indicates that the autocomplete textbox values can only be readable.

#### Default Value:  

* false

#### Example  

{% highlight html %}


<input type="text" id="visualmode" ej-autocomplete [dataSource]="language" [readOnly]="true" />

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.language = ['ActionScript', 'AppleScript', 'ASP', 'BASIC', 'BeanShell',
            'C', 'C++', 'C#', 'Clojure', 'COBOL', 'ColdFusion', 'DataFlex', 'DCL',
            'Erlang', 'E#', 'Fortran', 'F#', 'Flex', 'Google Apps Script', 'Groovy', 'Haskell', 'Hope', 'IBM HAScript',
            'Java', 'JavaScript', 'J#', 'Lisp', 'MATLAB', 'Oak', 'Perl', 'PHP',
            'Python', 'Ruby', 'Scala', 'Scheme', 'T-SQL', 'WebQL', 'ZOPL'];
    }
    
{% endhighlight %}

### selectValueByKey `number`
{:#members:selectvaluebykey}

Sets the value for the Autocomplete textbox based on the given input key value.

#### Example  

{% highlight html %}


<input type="text" id="searchbox" ej-autocomplete width="100%" [dataSource]="states" [fields]="fields" selectValueByKey="s5" />

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.fields = { key: 'index', text: 'countryName' };
        this.states = [
            { index: 's1', countryName: 'Alabama' }, { index: 's2', countryName: 'Alaska' },
            { index: 's3', countryName: 'Arizona' }, { index: 's4', countryName: 'Arkansas' },
            { index: 's5', countryName: 'California' }, { index: 's6', countryName: 'Colorado' },
            { index: 's20', countryName: 'Maryland' }, { index: 's21', countryName: 'Massachusetts' },
            { index: 's22', countryName: 'Michigan' }, { index: 's23', countryName: 'Montana' },
            { index: 's24', countryName: 'New Mexico' }, { index: '25', countryName: 'New York' },
            { index: '26', countryName: 'North Carolina' }, { index: 's27', countryName: 'Nevada' },
            { index: 's39', countryName: 'Vermont' }, { index: 's40', countryName: 'Virginia' },
            { index: 's41', countryName: 'Washington' }, { index: 's42', countryName: 'West Virginia' },
            { index: 's43', countryName: 'Wisconsin' }, { index: 's44', countryName: 'Wyoming' }
        ];

    }
    
{% endhighlight %}

### showEmptyResultText `boolean`
{:#members:showemptyresulttext}

Enables or disables showing the message when there are no suggestions for the entered text.

#### Default Value:  

* true

#### Example  

{% highlight html %}


<input type="text" id="visualmode" ej-autocomplete [dataSource]="language" [showEmptyResult]="false" />

{% endhighlight %}

{% highlight ts %}


    constructor() {
        this.language = ['ActionScript', 'AppleScript', 'ASP', 'BASIC', 'BeanShell',
            'C', 'C++', 'C#', 'Clojure', 'COBOL', 'ColdFusion', 'DataFlex', 'DCL',
            'Erlang', 'E#', 'Fortran', 'F#', 'Flex', 'Google Apps Script', 'Groovy', 'Haskell', 'Hope', 'IBM HAScript',
            'Java', 'JavaScript', 'J#', 'Lisp', 'MATLAB', 'Oak', 'Perl', 'PHP',
            'Python', 'Ruby', 'Scala', 'Scheme', 'T-SQL', 'WebQL', 'ZOPL'];
    }
    
{% endhighlight %}

### showLoadingIcon `boolean`
{:#members:showloadingicon}

Enables or disables the loading icon to intimate the searching operation. The loading icon is visible when there is a time delay to perform the search.

#### Default Value:  

* true

#### Example  

{% highlight html %}


<input id="databindingremote" type="text" ej-autocomplete width="100%" [query]="query" [fields]="fields" watermarkText="Search a customer" [dataSource]="dataManger" [showLoadingIcon]="false" />

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.fields = { text: 'ContactName', key: 'SupplierID' };
        this.dataManger = ej.DataManager({ url: 'http://js.syncfusion.com/ejServices/wcf/NorthWind.svc/', crossDomain: true }); // eslint-disable-line new-cap
        this.query = ej.Query().from('Suppliers').select('SupplierID', 'ContactName');
    }
    
{% endhighlight %}

### showPopupButton `boolean`
{:#members:showpopupbutton}

Enables the showPopup button in autocomplete textbox. When the showPopup button is clicked, it displays all the available data from the data source.

#### Default Value:  

* false

#### Example  

{% highlight html %}


<input type="text" id="visualmode" ej-autocomplete [dataSource]="language" [showPopupButton]="true" />

{% endhighlight %}

{% highlight ts %}


    constructor() {
        this.language = ['ActionScript', 'AppleScript', 'ASP', 'BASIC', 'BeanShell',
            'C', 'C++', 'C#', 'Clojure', 'COBOL', 'ColdFusion', 'DataFlex', 'DCL',
            'Erlang', 'E#', 'Fortran', 'F#', 'Flex', 'Google Apps Script', 'Groovy', 'Haskell', 'Hope', 'IBM HAScript',
            'Java', 'JavaScript', 'J#', 'Lisp', 'MATLAB', 'Oak', 'Perl', 'PHP',
            'Python', 'Ruby', 'Scala', 'Scheme', 'T-SQL', 'WebQL', 'ZOPL'];
    }
    
{% endhighlight %}

### showRoundedCorner `boolean`
{:#members:showroundedcorner}

Enables or disables rounded corner.

#### Default Value:  

* false

#### Example  

{% highlight html %}


<input type="text" id="visualmode" ej-autocomplete [dataSource]="language" [showRoundedCorner]="true" />

{% endhighlight %}

{% highlight ts %}


    constructor() {
        this.language = ['ActionScript', 'AppleScript', 'ASP', 'BASIC', 'BeanShell',
            'C', 'C++', 'C#', 'Clojure', 'COBOL', 'ColdFusion', 'DataFlex', 'DCL',
            'Erlang', 'E#', 'Fortran', 'F#', 'Flex', 'Google Apps Script', 'Groovy', 'Haskell', 'Hope', 'IBM HAScript',
            'Java', 'JavaScript', 'J#', 'Lisp', 'MATLAB', 'Oak', 'Perl', 'PHP',
            'Python', 'Ruby', 'Scala', 'Scheme', 'T-SQL', 'WebQL', 'ZOPL'];
    }
    
{% endhighlight %}

### showResetIcon `boolean`
{:#members:showreseticon}

Enables or disables reset icon to clear the textbox values.

#### Default Value:  

* false

#### Example  

{% highlight html %}


<input type="text" id="visualmode" ej-autocomplete [dataSource]="language" [showResetIcon]="true" />

{% endhighlight %}

{% highlight ts %}


    constructor() {
        this.language = ['ActionScript', 'AppleScript', 'ASP', 'BASIC', 'BeanShell',
            'C', 'C++', 'C#', 'Clojure', 'COBOL', 'ColdFusion', 'DataFlex', 'DCL',
            'Erlang', 'E#', 'Fortran', 'F#', 'Flex', 'Google Apps Script', 'Groovy', 'Haskell', 'Hope', 'IBM HAScript',
            'Java', 'JavaScript', 'J#', 'Lisp', 'MATLAB', 'Oak', 'Perl', 'PHP',
            'Python', 'Ruby', 'Scala', 'Scheme', 'T-SQL', 'WebQL', 'ZOPL'];
    }
    
{% endhighlight %}

### sortOrder `enum`
{:#members:sortorder}

<ts name = "ej.Autocomplete.SortOrder"/>

Sort order specifies whether the suggestion list values has to be displayed in ascending or descending order. 

<table>
<tr>
<th>Name<br/></th>
<th>Description<br/></th>
</tr>
<tr>
<td>Ascending<br/></td>
<td>Items to be displayed in the suggestion list in ascending order.<br/></td>
</tr>
<tr>
<td>Descending<br/></td>
<td>Items to be displayed in the suggestion list in descending order.<br/></td>
</tr>
</table>

{%seealso%} [SortOrder](https://help.syncfusion.com/api/js/global.html#SortOrder) {%endseealso%}

#### Default Value:  

* ej.SortOrder.Ascending

#### Example  

{% highlight html %}


<input type="text" id="visualmode" ej-autocomplete [dataSource]="language" sortOrder="descending" />

{% endhighlight %}

{% highlight ts %}


    constructor() {
        this.language = ['ActionScript', 'AppleScript', 'ASP', 'BASIC', 'BeanShell',
            'C', 'C++', 'C#', 'Clojure', 'COBOL', 'ColdFusion', 'DataFlex', 'DCL',
            'Erlang', 'E#', 'Fortran', 'F#', 'Flex', 'Google Apps Script', 'Groovy', 'Haskell', 'Hope', 'IBM HAScript',
            'Java', 'JavaScript', 'J#', 'Lisp', 'MATLAB', 'Oak', 'Perl', 'PHP',
            'Python', 'Ruby', 'Scala', 'Scheme', 'T-SQL', 'WebQL', 'ZOPL'];
    }
    
{% endhighlight %}

### template `string`
{:#members:template}

The template to display the suggestion list items with customized appearance.

#### Default Value:  

* null

#### Example  

{% highlight html %}


<input type="text" id="selectcountry" ej-autocomplete [dataSource]="countries" [template]="template" />

{% endhighlight %}

{% highlight ts %}


    constructor() {
        this.template = '<div class="flag ${sprite}"> </div><div class="txt"> ${text} </div>';
        this.countries = [
            { text: 'Algeria', sprite: 'flag-dz' }, { text: 'Argentina', sprite: 'flag-ar' },
            { text: 'Armenia', sprite: 'flag-am' }, { text: 'Brazil', sprite: 'flag-br' },
            { text: 'Bangladesh', sprite: 'flag-bd' }, { text: 'Canada', sprite: 'flag-ca' },
            { text: 'Cuba', sprite: 'flag-cu' }, { text: 'China', sprite: 'flag-cn' },
            { text: 'Denmark', sprite: 'flag-dk' }, { text: 'Estonia', sprite: 'flag-ee' }
        ];
    }
    
{% endhighlight %}

### validationMessage `Object`
{:#members:validationmessage}

The jQuery validation error message to be displayed on form validation.

#### Default Value:  

* null

#### Example  

{% highlight html %}


<input type="text" id="visualmode" ej-autocomplete [dataSource]="language" [validationRules]="Rules" [validationMessage]="msg" />

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.language = ['ActionScript', 'AppleScript', 'ASP', 'BASIC', 'BeanShell',
            'C', 'C++', 'C#', 'Clojure', 'COBOL', 'ColdFusion', 'DataFlex', 'DCL',
            'Erlang', 'E#', 'Fortran', 'F#', 'Flex', 'Google Apps Script', 'Groovy', 'Haskell', 'Hope', 'IBM HAScript',
            'Java', 'JavaScript', 'J#', 'Lisp', 'MATLAB', 'Oak', 'Perl', 'PHP',
            'Python', 'Ruby', 'Scala', 'Scheme', 'T-SQL', 'WebQL', 'ZOPL'];
        this.Rules: [{ 



required: true 


}] 


this.msg: [{ 



required: "Enter some value" 


}]
    }
    
{% endhighlight %}

### validationRules `Object`
{:#members:validationrules}

The jQuery validation rules for form validation.

#### Default Value:  

* null

#### Example  

VALIDATIONRULES
{% highlight html %}


<input type="text" id="visualmode" ej-autocomplete [dataSource]="language" [validationRules]="Rules" [validationMessage]="msg" />

{% endhighlight %}

{% highlight ts %}


    constructor() {
        this.language = ['ActionScript', 'AppleScript', 'ASP', 'BASIC', 'BeanShell',
            'C', 'C++', 'C#', 'Clojure', 'COBOL', 'ColdFusion', 'DataFlex', 'DCL',
            'Erlang', 'E#', 'Fortran', 'F#', 'Flex', 'Google Apps Script', 'Groovy', 'Haskell', 'Hope', 'IBM HAScript',
            'Java', 'JavaScript', 'J#', 'Lisp', 'MATLAB', 'Oak', 'Perl', 'PHP',
            'Python', 'Ruby', 'Scala', 'Scheme', 'T-SQL', 'WebQL', 'ZOPL'];
       this.Rules: [{ 



required: true 


}] 


this.msg: [{ 



required: "Enter some value" 


}]
    }
    
{% endhighlight %}

### value `string`
{:#members:value}

The value to be displayed in the autocomplete textbox.

#### Default Value:  

* null

#### Example  

{% highlight html %}


<input type="text" id="visualmode" ej-autocomplete [dataSource]="language" [value]="value" />

{% endhighlight %}

{% highlight ts %}


    constructor() {
        this.language = ['ActionScript', 'AppleScript', 'ASP', 'BASIC', 'BeanShell',
            'C', 'C++', 'C#', 'Clojure', 'COBOL', 'ColdFusion', 'DataFlex', 'DCL',
            'Erlang', 'E#', 'Fortran', 'F#', 'Flex', 'Google Apps Script', 'Groovy', 'Haskell', 'Hope', 'IBM HAScript',
            'Java', 'JavaScript', 'J#', 'Lisp', 'MATLAB', 'Oak', 'Perl', 'PHP',
            'Python', 'Ruby', 'Scala', 'Scheme', 'T-SQL', 'WebQL', 'ZOPL'];
        this.value = "Perl"
    }
    
{% endhighlight %}

### visible `boolean`
{:#members:visible}

Enables or disables the visibility of the autocomplete textbox.

#### Default Value:  

* true

#### Example  

{% highlight html %}


<input type="text" id="visualmode" ej-autocomplete [dataSource]="language" [visible]="true" />

{% endhighlight %}

{% highlight ts %}


    constructor() {
        this.language = ['ActionScript', 'AppleScript', 'ASP', 'BASIC', 'BeanShell',
            'C', 'C++', 'C#', 'Clojure', 'COBOL', 'ColdFusion', 'DataFlex', 'DCL',
            'Erlang', 'E#', 'Fortran', 'F#', 'Flex', 'Google Apps Script', 'Groovy', 'Haskell', 'Hope', 'IBM HAScript',
            'Java', 'JavaScript', 'J#', 'Lisp', 'MATLAB', 'Oak', 'Perl', 'PHP',
            'Python', 'Ruby', 'Scala', 'Scheme', 'T-SQL', 'WebQL', 'ZOPL'];
    }
    
{% endhighlight %}

### watermarkText `string`
{:#members:watermarktext}

The text to be displayed when the value of the autocomplete textbox is empty.

#### Default Value:  

* null

#### Example  

{% highlight html %}


<input type="text" id="visualmode" ej-autocomplete watermarkText="Select skills" [dataSource]="language" />

{% endhighlight %}

{% highlight ts %}


    constructor() {
        this.language = ['ActionScript', 'AppleScript', 'ASP', 'BASIC', 'BeanShell',
            'C', 'C++', 'C#', 'Clojure', 'COBOL', 'ColdFusion', 'DataFlex', 'DCL',
            'Erlang', 'E#', 'Fortran', 'F#', 'Flex', 'Google Apps Script', 'Groovy', 'Haskell', 'Hope', 'IBM HAScript',
            'Java', 'JavaScript', 'J#', 'Lisp', 'MATLAB', 'Oak', 'Perl', 'PHP',
            'Python', 'Ruby', 'Scala', 'Scheme', 'T-SQL', 'WebQL', 'ZOPL'];
    }
    
{% endhighlight %}

### width `string|number`
{:#members:width}

The width of the Autocomplete textbox.

#### Default Value:  

* null

#### Example  

{% highlight html %}


<input type="text" id="visualmode" ej-autocomplete width="100%" [dataSource]="language" />

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.language = ['ActionScript', 'AppleScript', 'ASP', 'BASIC', 'BeanShell',
            'C', 'C++', 'C#', 'Clojure', 'COBOL', 'ColdFusion', 'DataFlex', 'DCL',
            'Erlang', 'E#', 'Fortran', 'F#', 'Flex', 'Google Apps Script', 'Groovy', 'Haskell', 'Hope', 'IBM HAScript',
            'Java', 'JavaScript', 'J#', 'Lisp', 'MATLAB', 'Oak', 'Perl', 'PHP',
            'Python', 'Ruby', 'Scala', 'Scheme', 'T-SQL', 'WebQL', 'ZOPL'];
    }
    
{% endhighlight %}

## Methods

### clearText()
{:#methods:cleartext}

Clears the text in the Autocomplete textbox.

N> This method does not accept any arguments.

#### Example  

{% highlight html %}


<input type="text" id="autocompletecomp" ej-autocomplete />

{% endhighlight %}

{% highlight ts %}

    let acObj = $('#autocompletecomp').data('ejAutocomplete');
    acObj.clearText();
    
{% endhighlight %}

### destroy()
{:#methods:destroy}

Destroys the Autocomplete widget.

N> This method does not accept any arguments.

#### Example  

{% highlight html %}


<input type="text" id="autocompletecomp" ej-autocomplete />

{% endhighlight %}

{% highlight ts %}

    let acObj = $('#autocompletecomp').data('ejAutocomplete');
    acObj.destroy();
    
{% endhighlight %}

### disable()
{:#methods:disable}

Disables the autocomplete widget.

N> This method does not accept any arguments.

#### Example  

{% highlight html %}


<input type="text" id="autocompletecomp" ej-autocomplete />

{% endhighlight %}

{% highlight ts %}

    let acObj = $('#autocompletecomp').data('ejAutocomplete');
    acObj.disable();
    
{% endhighlight %}

### enable()
{:#methods:enable}

Enables the autocomplete widget.

N> This method does not accept any arguments.

#### Example  

{% highlight html %}


<input type="text" id="autocompletecomp" ej-autocomplete />

{% endhighlight %}

{% highlight ts %}

    let acObj = $('#autocompletecomp').data('ejAutocomplete');
    acObj.enable();
    
{% endhighlight %}

### getSelectedItems()
{:#methods:getselecteditems}

Returns objects (data object) of all the selected items in the autocomplete textbox.

N> This method does not accept any arguments.

#### Returns: object

#### Example  

{% highlight html %}


<input type="text" id="autocompletecomp" ej-autocomplete />

{% endhighlight %}

{% highlight ts %}

    let acObj = $('#autocompletecomp').data('ejAutocomplete');
    acObj.getSelectedItems();
    
{% endhighlight %}

### getValue()
{:#methods:getvalue}

Returns the current selected value from the Autocomplete textbox.

N> This method does not accept any arguments.

#### Returns: string

#### Example  

{% highlight html %}


<input type="text" id="autocompletecomp" ej-autocomplete />

{% endhighlight %}

{% highlight ts %}

    let acObj = $('#autocompletecomp').data('ejAutocomplete');
    acObj.getValue();
    
{% endhighlight %}

### getActiveText()
{:#methods:getactivetext}

Returns the current active text value in the Autocomplete suggestion list.

N> This method does not accept any arguments.

#### Returns: string

#### Example  

{% highlight html %}


<input type="text" id="autocompletecomp" ej-autocomplete />

{% endhighlight %}

{% highlight ts %}

    let acObj = $('#autocompletecomp').data('ejAutocomplete');
    acObj.getActiveText();
    
{% endhighlight %}


### search()
{:#methods:search}

Search the entered text and show it in the suggestion list if available.

N> This method does not accept any arguments.

#### Example  

{% highlight html %}


<input type="text" id="autocompletecomp" ej-autocomplete />

{% endhighlight %}

{% highlight ts %}

    let acObj = $('#autocompletecomp').data('ejAutocomplete');
    acObj.search();
    
{% endhighlight %}

### open()
{:#methods:open}

Open up the autocomplete suggestion popup with all list items.

N> This method does not accept any arguments.

#### Example  

{% highlight html %}


<input type="text" id="autocompletecomp" ej-autocomplete />

{% endhighlight %}

{% highlight ts %}

    let acObj = $('#autocompletecomp').data('ejAutocomplete');
    acObj.open();
    
{% endhighlight %}

### selectValueByKey(key)
{:#methods:selectvaluebykey}

Sets the value of the Autocomplete textbox based on the given key value.

<table>
<tr>
<th>Name<br/></th>
<th>Type<br/></th>
<th>Description<br/></th>
</tr>
<tr>
<td>Key<br/></td>
<td>string<br/></td>
<td>The key value of the specific suggestion item.<br/></td>
</tr>
</table>

 N>  This method accepts string as an argument.

#### Example  

{% highlight html %}


<input type="text" id="autocompletecomp" ej-autocomplete />

{% endhighlight %}

{% highlight ts %}

    let acObj = $('#autocompletecomp').data('ejAutocomplete');
    acObj.selectValueByKey("key value");
    
{% endhighlight %}

### selectValueByText(text)
{:#methods:selectvaluebytext}

Sets the value of the Autocomplete textbox based on the given input text value.

<table>
<tr>
<th>Name<br/></th>
<th>Type<br/></th>
<th>Description<br/></th>
</tr>
<tr>
<td>Text<br/></td>
<td>string<br/></td>
<td>The text (label) value of the specific suggestion item.<br/></td>
</tr>
</table>

#### Example  

{% highlight html %}


<input type="text" id="autocompletecomp" ej-autocomplete />

{% endhighlight %}

{% highlight ts %}

    let acObj = $('#autocompletecomp').data('ejAutocomplete');
    acObj.selectValueByText("text");
    
{% endhighlight %}

## Events

### actionBegin
{:#events:actionBegin}

Triggers when the AJAX requests Begins.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the Autocomplete model</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the name of the event</td>
</tr>
</tbody>
</table>

 N>  It internally uses jQuery ajaxStart event. For details refer [here](http://api.jquery.com/ajaxStart/#).

#### Example

{% highlight html %}


<input id="databindingremote" type="text" ej-autocomplete width="100%" [query]="query" [fields]="fields" watermarkText="Search a customer" [dataSource]="dataManger" (actionBegin)="actionbegin(args)" />

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.fields = { text: 'ContactName', key: 'SupplierID' };
        this.dataManger = ej.DataManager({ url: 'http://js.syncfusion.com/ejServices/wcf/NorthWind.svc/', crossDomain: true }); // eslint-disable-line new-cap
        this.query = ej.Query().from('Suppliers').select('SupplierID', 'ContactName');

    }
    actionbegin(args) {
        // Your code here
    }
    
{% endhighlight %}

### actionSuccess
{:#events:actionsuccess}

Triggers when the data requested from AJAX will get successfully loaded in the **Autocomplete** widget. 

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
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">count</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns number of times trying to fetch the data</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the Autocomplete model</td>
</tr>
<tr>
<td class="name">query</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the query for data retrieval </td>
</tr>
<tr>
<td class="name">request</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the query for data retrieval from the Database </td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">result</td>
<td class="type"><span class="param-type">array</span></td>
<td class="description">Returns the number of items fetched from remote data</td>
</tr>
<tr>
<td class="name">xhr</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the requested data</td>
</tr>
</tbody>
</table>

 N>  It internally uses jQuery ajaxSuccess event. For details refer [here](http://api.jquery.com/ajaxsuccess/#).

#### Example

{% highlight html %}


<input id="databindingremote" type="text" ej-autocomplete width="100%" [query]="query" [fields]="fields" watermarkText="Search a customer" [dataSource]="dataManger" (actionSuccess)="actionsuccess(args)" />

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.fields = { text: 'ContactName', key: 'SupplierID' };
        this.dataManger = ej.DataManager({ url: 'http://js.syncfusion.com/ejServices/wcf/NorthWind.svc/', crossDomain: true }); // eslint-disable-line new-cap
        this.query = ej.Query().from('Suppliers').select('SupplierID', 'ContactName');

    }
    actionsuccess(args) {
        // Your code here
    }

{% endhighlight %}

### actionComplete
{:#events:actioncomplete}

Triggers when the AJAX requests complete. The request may get failed or succeed.

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
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">count</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns number of times trying to fetch the data</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the Autocomplete model</td>
</tr>
<tr>
<td class="name">query</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the query for data retrieval </td>
</tr>
<tr>
<td class="name">request</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the query for data retrieval from the Database </td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">result</td>
<td class="type"><span class="param-type">array</span></td>
<td class="description">Returns the number of items fetched from remote data</td>
</tr>
<tr>
<td class="name">xhr</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the requested data</td>
</tr>
</tbody>
</table>

N> It internally uses jQuery ajaxComplete event. For details refer [here](http://api.jquery.com/ajaxcomplete/#).

#### Example

{% highlight html %}


<input id="databindingremote" type="text" ej-autocomplete width="100%" [query]="query" [fields]="fields" watermarkText="Search a customer" [dataSource]="dataManger" (actionComplete)="actioncomplete(args)" />

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.fields = { text: 'ContactName', key: 'SupplierID' };
        this.dataManger = ej.DataManager({ url: 'http://js.syncfusion.com/ejServices/wcf/NorthWind.svc/', crossDomain: true }); // eslint-disable-line new-cap
        this.query = ej.Query().from('Suppliers').select('SupplierID', 'ContactName');

    }
    actioncomplete(args) {
        // Your code here
    }

{% endhighlight %}

### actionFailure
{:#events:actionfailure}

Triggers when the data requested from AJAX get failed.

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
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">error</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the error message</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the Autocomplete model</td>
</tr>
<tr>
<td class="name">query</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the query for data retrieval </td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
</tbody>
</table>

 N>  It internally uses jQuery ajaxError event. For details refer [here](http://api.jquery.com/ajaxerror/#).

#### Example

{% highlight html %}


<input id="databindingremote" type="text" ej-autocomplete width="100%" [query]="query" [fields]="fields" watermarkText="Search a customer" [dataSource]="dataManger" (actionFailure)="actionfailure(args)" />

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.fields = { text: 'ContactName', key: 'SupplierID' };
        this.dataManger = ej.DataManager({ url: 'http://js.syncfusion.com/ejServices/wcf/NorthWind.svc/ds', crossDomain: true }); // eslint-disable-line new-cap
        this.query = ej.Query().from('Suppliers').select('SupplierID', 'ContactName');

    }
    actionfailure(args) {
        // Your code here
    }

{% endhighlight %}

### change
{:#events:change}

Triggers when the text box value is changed.

<table>
<tr>
<th>Name<br/></th>
<th>Type<br/></th>
<th>Description<br/></th>
</tr>
<tr>
<td>cancel<br/></td>
<td>boolean<br/></td>
<td>Set this option to true to cancel the event.<br/></td>
</tr>
<tr>
<td>model<br/></td>
<td><ts ref="ej.Autocomplete.Model"/>Object<br/></td>
<td>Instance of the autocomplete model object.<br/></td>
</tr>
<tr>
<td>type<br/></td>
<td>string<br/></td>
<td>Name of the event.<br/></td>
</tr>
<tr>
<td>value<br/></td>
<td>string<br/></td>
<td>Value of the autocomplete textbox.<br/></td>
</tr>
</table>

#### Example  

{% highlight html %}


<input id="databindingremote" type="text" ej-autocomplete width="100%" [query]="query" [fields]="fields" watermarkText="Search a customer" [dataSource]="dataManger" (ejchange)="onchange(args)" />

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.fields = { text: 'ContactName', key: 'SupplierID' };
        this.dataManger = ej.DataManager({ url: 'http://js.syncfusion.com/ejServices/wcf/NorthWind.svc/', crossDomain: true }); // eslint-disable-line new-cap
        this.query = ej.Query().from('Suppliers').select('SupplierID', 'ContactName');

    }
    onchange(args) {
        // Your code here
    }

{% endhighlight %}

### close
{:#events:close}

Triggers after the suggestion popup is closed.

<table>
<tr>
<th>Name<br/></th>
<th>Type<br/></th>
<th>Description<br/></th>
</tr>
<tr>
<td>cancel<br/></td>
<td>boolean<br/></td>
<td>Set this option to true to cancel the event.<br/></td>
</tr>
<tr>
<td>model<br/></td>
<td><ts ref="ej.Autocomplete.Model"/>Object<br/></td>
<td>Instance of the autocomplete model object.<br/></td>
</tr>
<tr>
<td>type<br/></td>
<td>string<br/></td>
<td>Name of the event.<br/></td>
</tr>
</table>

#### Example  

{% highlight html %}


<input id="databindingremote" type="text" ej-autocomplete width="100%" [query]="query" [fields]="fields" watermarkText="Search a customer" [dataSource]="dataManger" (close)="onclose(args)" />

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.fields = { text: 'ContactName', key: 'SupplierID' };
        this.dataManger = ej.DataManager({ url: 'http://js.syncfusion.com/ejServices/wcf/NorthWind.svc/', crossDomain: true }); // eslint-disable-line new-cap
        this.query = ej.Query().from('Suppliers').select('SupplierID', 'ContactName');

    }
    onclose(args) {
        // Your code here
    }

{% endhighlight %}

### create
{:#events:create}

Triggers when Autocomplete widget is created.

<table>
<tr>
<th>Name<br/></th>
<th>Type<br/></th>
<th>Description<br/></th>
</tr>
<tr>
<td>cancel<br/></td>
<td>boolean<br/></td>
<td>Set this option to true to cancel the event.<br/></td>
</tr>
<tr>
<td>model<br/></td>
<td><ts ref="ej.Autocomplete.Model"/>Object<br/></td>
<td>Instance of the autocomplete model object.<br/></td>
</tr>
<tr>
<td>type<br/></td>
<td>string<br/></td>
<td>Name of the event.<br/></td>
</tr>
</table>

#### Example  

{% highlight html %}


<input id="databindingremote" type="text" ej-autocomplete width="100%" [query]="query" [fields]="fields" watermarkText="Search a customer" [dataSource]="dataManger" (create)="oncreate(args)" />

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.fields = { text: 'ContactName', key: 'SupplierID' };
        this.dataManger = ej.DataManager({ url: 'http://js.syncfusion.com/ejServices/wcf/NorthWind.svc/', crossDomain: true }); // eslint-disable-line new-cap
        this.query = ej.Query().from('Suppliers').select('SupplierID', 'ContactName');

    }
    oncreate(args) {
        // Your code here
    }
    
{% endhighlight %}

### destroy
{:#events:destroy}

Triggers after the Autocomplete widget is destroyed.

<table>
<tr>
<th>Name<br/></th>
<th>Type<br/></th>
<th>Description<br/></th>
</tr>
<tr>
<td>cancel<br/></td>
<td>boolean<br/></td>
<td>Set this option to true to cancel the event.<br/></td>
</tr>
<tr>
<td>model<br/></td>
<td><ts ref="ej.Autocomplete.Model"/>Object<br/></td>
<td>Instance of the autocomplete model object.<br/></td>
</tr>
<tr>
<td>type<br/></td>
<td>string<br/></td>
<td>Name of the event.<br/></td>
</tr>
</table>

#### Example  

{% highlight html %}


<input id="databindingremote" type="text" ej-autocomplete width="100%" [query]="query" [fields]="fields" watermarkText="Search a customer" [dataSource]="dataManger" (destroy)="ondestroy(args)" />

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.fields = { text: 'ContactName', key: 'SupplierID' };
        this.dataManger = ej.DataManager({ url: 'http://js.syncfusion.com/ejServices/wcf/NorthWind.svc/', crossDomain: true }); // eslint-disable-line new-cap
        this.query = ej.Query().from('Suppliers').select('SupplierID', 'ContactName');

    }
    ondestroy(args) {
        // Your code here
    }    

{% endhighlight %}

### focusIn
{:#events:focusin}

Triggers after the autocomplete textbox is focused.

<table>
<tr>
<th>Name<br/></th>
<th>Type<br/></th>
<th>Description<br/></th>
</tr>
<tr>
<td>cancel<br/></td>
<td>boolean<br/></td>
<td>Set this option to true to cancel the event.<br/></td>
</tr>
<tr>
<td>model<br/></td>
<td><ts ref="ej.Autocomplete.Model"/>Object<br/></td>
<td>Instance of the autocomplete model object.<br/></td>
</tr>
<tr>
<td>type<br/></td>
<td>string<br/></td>
<td>Name of the event.<br/></td>
</tr>
<tr>
<td>value<br/></td>
<td>string<br/></td>
<td>Value of the autocomplete textbox.<br/></td>
</tr>
</table>

#### Example  

{% highlight html %}


<input id="databindingremote" type="text" ej-autocomplete width="100%" [query]="query" [fields]="fields" watermarkText="Search a customer" [dataSource]="dataManger" (focusIn)="onfocusin(args)" />

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.fields = { text: 'ContactName', key: 'SupplierID' };
        this.dataManger = ej.DataManager({ url: 'http://js.syncfusion.com/ejServices/wcf/NorthWind.svc/', crossDomain: true }); // eslint-disable-line new-cap
        this.query = ej.Query().from('Suppliers').select('SupplierID', 'ContactName');

    }
    onfocusin(args) {
        // Your code here
    }
    
{% endhighlight %}

### focusOut
{:#events:focusout}

Triggers after the Autocomplete textbox gets out of the focus.

<table>
<tr>
<th>Name<br/></th>
<th>Type<br/></th>
<th>Description<br/></th>
</tr>
<tr>
<td>cancel<br/></td>
<td>boolean<br/></td>
<td>Set this option to true to cancel the event.<br/></td>
</tr>
<tr>
<td>model<br/></td>
<td><ts ref="ej.Autocomplete.Model"/>Object<br/></td>
<td>Instance of the autocomplete model object.<br/></td>
</tr>
<tr>
<td>type<br/></td>
<td>string<br/></td>
<td>Name of the event.<br/></td>
</tr>
<tr>
<td>value<br/></td>
<td>string<br/></td>
<td>Value of the autocomplete textbox.<br/></td>
</tr>
</table>

#### Example  

{% highlight html %}


<input id="databindingremote" type="text" ej-autocomplete width="100%" [query]="query" [fields]="fields" watermarkText="Search a customer" [dataSource]="dataManger" (focusOut)="onfocusout(args)" />

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.fields = { text: 'ContactName', key: 'SupplierID' };
        this.dataManger = ej.DataManager({ url: 'http://js.syncfusion.com/ejServices/wcf/NorthWind.svc/', crossDomain: true }); // eslint-disable-line new-cap
        this.query = ej.Query().from('Suppliers').select('SupplierID', 'ContactName');

    }
    onfocusout(args) {
        // Your code here
    }
    
{% endhighlight %}

### open
{:#events:open}

Triggers after the suggestion list is opened.

<table>
<tr>
<th>Name<br/></th>
<th>Type<br/></th>
<th>Description<br/></th>
</tr>
<tr>
<td>cancel<br/></td>
<td>boolean<br/></td>
<td>Set this option to true to cancel the event.<br/></td>
</tr>
<tr>
<td>model<br/></td>
<td><ts ref="ej.Autocomplete.Model"/>Object<br/></td>
<td>Instance of the autocomplete model object.<br/></td>
</tr>
<tr>
<td>type<br/></td>
<td>string<br/></td>
<td>Name of the event.<br/></td>
</tr>
</table>

#### Example  

{% highlight html %}


<input id="databindingremote" type="text" ej-autocomplete width="100%" [query]="query" [fields]="fields" watermarkText="Search a customer" [dataSource]="dataManger" (open)="onopen(args)" />

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.fields = { text: 'ContactName', key: 'SupplierID' };
        this.dataManger = ej.DataManager({ url: 'http://js.syncfusion.com/ejServices/wcf/NorthWind.svc/', crossDomain: true }); // eslint-disable-line new-cap
        this.query = ej.Query().from('Suppliers').select('SupplierID', 'ContactName');

    }
    onopen(args) {
        // Your code here
    }
    
{% endhighlight %}

### select
{:#events:select}

Triggers when an item has been selected from the suggestion list.

<table>
<tr>
<th>Name<br/></th>
<th>Type<br/></th>
<th>Description<br/></th>
</tr>
<tr>
<td>cancel<br/></td>
<td>boolean<br/></td>
<td>Set this option to true to cancel the event.<br/></td>
</tr>
<tr>
<td>model<br/></td>
<td><ts ref="ej.Autocomplete.Model"/>Object<br/></td>
<td>Instance of the autocomplete model object.<br/></td>
</tr>
<tr>
<td>type<br/></td>
<td>string<br/></td>
<td>Name of the event.<br/></td>
</tr>
<tr>
<td>value<br/></td>
<td>string<br/></td>
<td>Value of the autocomplete textbox.<br/></td>
</tr>
<tr>
<td>text<br/></td>
<td>string<br/></td>
<td>Text of the selected item.<br/></td>
</tr>
<tr>
<td>key<br/></td>
<td>string<br/></td>
<td>Key of the selected item.<br/></td
></tr>
<tr>
<td>Item<br/></td>
<td><ts ref="ej.Autocomplete.Model"/>Object<br/></td>
<td>Data object of the selected item.<br/></td>
</tr>
</table>

#### Example  

{% highlight html %}


<input id="databindingremote" type="text" ej-autocomplete width="100%" [query]="query" [fields]="fields" watermarkText="Search a customer" [dataSource]="dataManger" (select)="onselect(args)" />

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.fields = { text: 'ContactName', key: 'SupplierID' };
        this.dataManger = ej.DataManager({ url: 'http://js.syncfusion.com/ejServices/wcf/NorthWind.svc/', crossDomain: true }); // eslint-disable-line new-cap
        this.query = ej.Query().from('Suppliers').select('SupplierID', 'ContactName');

    }
    onselect(args) {
        // Your code here
    }
    
{% endhighlight %}
