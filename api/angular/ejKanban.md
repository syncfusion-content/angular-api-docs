---
layout: post
title: Properties, Methods and Events of Essential Angular Kanban Widget
description: Members,Methods,Events available in Kanban
documentation: API
platform: angular-api
keywords: Kanban, API, Essential Angular Kanban
---

# ejKanban

The Kanban can be easily configured to the DOM element, such as div. You can create a Kanban with a highly customizable look and feel.


#### Example


{% highlight html %}
<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status">
 <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
 </e-kanban-columns>
</ej-kanban>
{% endhighlight %}

{% highlight ts %}

export class KanbanComponent {
    
    public  kanbanData:any;

        constructor()
        {
                 this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }]; 
        }
}

{% endhighlight %}

#### Requires
{:.require}

* module:jQuery
* module:jsrender.min.js
* module:ej.globalize.min.js
* module:ej.core.min.js
* module:ej.data.min.js
* module:ej.touch.min.js
* module:ej.draggable.min.js
* module:ej.kanban.min.js
* module:ej.scroller.min.js
* module:ej.waitingpopup.min.js
* module:ej.button.min.js
* module:ej.dialog.min.js
* module:ej.dropdownlist.min.js
* module:ej.datepicker.min.js
* module:ej.datetimepicker.min.js
* module:ej.editor.min.js
* module:ej.checkbox.min.js
* module:ej.tab.min.js
* module:ej.splitbutton.js
* module:ej.rte.min.js
* module:ej.toolbar.min.js
* module:ej.menu.min.js

## Members

### allowDragAndDrop `boolean`
{:#members:allowdraganddrop}

Gets or sets a value that indicates whether to enable allowDragAndDrop behavior on Kanban.

#### Default Value

* true

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" allowDragAndDrop="true" keyField="Status" fields.content="Summary" fields.primaryKey="Id">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
               this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
    }
	
{% endhighlight %}


### allowTitle `boolean`
{:#members:allowtitle}

To enable or disable the title of the card.

#### Default Value:

* false

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" allowTitle="true" keyField="Status" fields.content="Summary" fields.primaryKey="Id">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
              this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
    }
    
{% endhighlight %}


### swimlaneSettings `Object`
{:#members:swimlanesettings}

Customize the settings for swim lane.

#### Default Value:

* Object

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id" fields.swimlaneKey="Assignee">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
               this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
    }
    
{% endhighlight %}


### swimlaneSettings.showCount `boolean`
{:#members:swimlanesettings-showcount}

To enable or disable items count in swim lane.

#### Default Value:

* true

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id" fields.swimlaneKey="Assignee" swimlaneSettings.showCount="true">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
              this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
    }
    
{% endhighlight %}


### swimlaneSettings.allowDragAndDrop `boolean`
{:#members:swimlanesettings-allowdraganddrop}

To enable or disable DragAndDrop across swim lane.

#### Default Value:

* false

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id" fields.swimlaneKey="Assignee" swimlaneSettings.allowDragAndDrop="true">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
               this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
    }
    
{% endhighlight %}


### swimlaneSettings.unassignedGroup `Object`
{:#members:swimlanesettings-unassignedgroup}

Customize the settings for unassigned category of swim lane.

#### Default Value:

* Object

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id" fields.swimlaneKey="Assignee" [swimlaneSettings.unassignedGroup.enable]="true">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
              this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
    }
    
{% endhighlight %}


### swimlaneSettings.unassignedGroup.enable `boolean`
{:#members:swimlanesettings-unassignedgroup-enable}

To enable or disable unassigned category change with swim lane key values.

#### Default Value:

* true

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id" fields.swimlaneKey="Assignee" [swimlaneSettings.unassignedGroup.enable]="true">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
               this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
    }
    
{% endhighlight %}


### swimlaneSettings.unassignedGroup.keys `Array`
{:#members:swimlanesettings-unassignedgroup-keys}

To set the user defined values which are need to categorized as unassigned category swim lane groups.

#### Default Value:

* ["null","undefined",""]

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id" fields.swimlaneKey="Assignee" [swimlaneSettings.unassignedGroup.keys]="key">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
		this.key = ["Andrew Fuller", "", "null"];
	}
    
{% endhighlight %}


### allowToggleColumn `boolean`
{:#members:allowtogglecolumn}

To enable or disable the column expand /collapse.

#### Default Value:

* false

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" allowToggleColumn="true" keyField="Status" fields.content="Summary" fields.primaryKey="Id">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
    }
    
{% endhighlight %}


### allowSearching `boolean`
{:#members:allowsearching}

To enable Searching operation in Kanban.

#### Default Value:

* false

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" allowSearching="true" keyField="Status" fields.content="Summary" fields.primaryKey="Id">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
    }
    
{% endhighlight %}


### allowFiltering `boolean`
{:#members:allowfiltering}

To enable filtering behavior on Kanban.User can specify query in filterSettings collection after enabling allowFiltering.

#### Default Value:

* false

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" allowFiltering="true" keyField="Status" fields.content="Summary" fields.primaryKey="Id" [filterSettings]="filterSetting">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}
     
	constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
        this.filterSetting = [
            { text: "Janet Issues", query: new ej.Query().where("Assignee",ej.FilterOperators.equal, "Janet Leverling"), description: "Displays issues which matches the assignee as 'Janet Leverling'" },
            { text: "Closed Issues", query: new ej.Query().where("Status",ej.FilterOperators.equal, "Close"), description: "Display the 'Closed' issues" }
        ];
	}
    
{% endhighlight %}


### allowSelection `boolean`
{:#members:allowselection}

Gets or sets a value that indicates whether to enable allowSelection behavior on Kanban.User can select card and the selected card will be highlighted on Kanban.

#### Default Value:

* true

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" allowSelection="true" keyField="Status" fields.content="Summary" fields.primaryKey="Id">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	}
    
{% endhighlight %}


### allowHover `boolean`
{:#members:allowhover}

Gets or sets a value that indicates whether to allow card hover actions.

#### Default Value

* true

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" allowHover="true" keyField="Status" fields.content="Summary" fields.primaryKey="Id">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	}
    
{% endhighlight %}


### allowKeyboardNavigation `boolean`
{:#members:allowkeyboardnavigation}

To allow keyboard navigation actions.

#### Default Value

* false

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" allowKeyboardNavigation="true" keyField="Status" fields.content="Summary" fields.primaryKey="Id">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	}
    
{% endhighlight %}


### allowScrolling `boolean`
{:#members:allowscrolling}

Gets or sets a value that indicates whether to enable the scrollbar in the Kanban and view the card by scroll through the Kanban manually.

#### Default Value

* false

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" allowScrolling="true" keyField="Status" fields.content="Summary" fields.primaryKey="Id" fields.swimlaneKey="Assignee" [scrollSettings]="scrollSetting">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
		this.scrollSetting = {
            width: 700,
            height: 400
        }
	}
    
{% endhighlight %}


### allowPrinting `boolean`
{:#members:allowprinting}

Gets or sets a value that indicates whether to enable printing option.

#### Default Value:

* false

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" allowPrinting="true" keyField="Status" fields.content="Summary" fields.primaryKey="Id">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	}
    
{% endhighlight %}


### contextMenuSettings `Object`
{:#members:contextmenusettings}

Gets or sets an object that indicates whether to customize the context menu behavior of the Kanban.

#### Default Value:

* Object

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id" [contextMenuSettings.enable]="true">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	}
    
{% endhighlight %}


### contextMenuSettings.enable `boolean`
{:#members:contextmenusettings-enable}

To enable context menu.All default context menu will show.

#### Default Value:

* false

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id" [contextMenuSettings.enable]="true">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	}
    
{% endhighlight %}


### contextMenuSettings.disableDefaultItems `Array`
{:#members:contextmenusettings-disabledefaultitems}

Gets or sets a value that indicates the list of items needs to be disable from default context menu items.

#### Default Value:

* Array

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id" [contextMenuSettings]="contextMenuSetting">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
		this.contextMenuSetting =  {
                enable: true,
                disableDefaultItems: [ej.Kanban.MenuItem.MoveLeft]
        };
	}
    
{% endhighlight %}


### contextMenuSettings.menuItems `Array`
{:#members:contextmenusettings-menuitems}

Its used to add specific default context menu items.

#### Default Value:

* Array

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id" [contextMenuSettings]="contextMenuSetting">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
		this.contextMenuSetting =  {
                enable: true,
                menuItems:["Move Right","Move Left"]
        };
	}
    
{% endhighlight %}


### contextMenuSettings.customMenuItems `Array`
{:#members:contextmenusettings-custommenuitems}

Gets or sets a value that indicates whether to add custom contextMenu items. 

#### Default Value:

* Array

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id" [contextMenuSettings]="contextMenuSetting">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
		this.contextMenuSetting = {
                enable: true,
                customMenuItems: [
                          { text: "Menu1" },
                          { text: "Menu2", target: ej.Kanban.Target.Header }                          
                ]
        };
	}
    
{% endhighlight %}


### contextMenuSettings.customMenuItems.target `enum`
{:#members:contextmenusettings-custommenuitems-target}

<ts name="ej.Kanban.Target"/>

Its sets target element to custom context menu item.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">Header</td>
<td class="description">Sets context menu to Kanban header</td>
</tr>
<tr>
<td class="name">Content</td>
<td class="description">Sets context menu to Kanban content</td>
</tr>
<tr>
<td class="name">Card</td>
<td class="description">Sets context menu to Kanban card</td>
</tr>
<tr>
<td class="name">All</td>
<td class="description">Sets context menu to Kanban</td>
</tr>
</tbody>
</table>

#### Default Value

* ej.Kanban.Target.All

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id" [contextMenuSettings]="contextMenuSetting">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
		this.contextMenuSetting = {
                enable: true,
                customMenuItems: [
                          { text: "Menu1", target: ej.Kanban.Target.Card },
                          { text: "Menu2", target: ej.Kanban.Target.Header }
                ]
        };
	}
    
{% endhighlight %}


### contextMenuSettings.customMenuItems.text `string`
{:#members:contextmenusettings-custommenuitems-text}

Gets the display name to custom menu item.

#### Default Value:

* null

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id" [contextMenuSettings]="contextMenuSetting">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
		this.contextMenuSetting = {
                enable: true,
                customMenuItems: [
                          { text: "Menu1" },
                          { text: "Menu2" }
                ]
        };
	}
    
{% endhighlight %}


### contextMenuSettings.customMenuItems.template `string`
{:#members:contextmenusettings-custommenuitems-template}

Gets the template to render custom context menu item.

#### Default Value:

* null

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id" [contextMenuSettings]="contextMenuSetting">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>
	<ul id="template">
        <li><a>Backlog</a></li>
        <li><a>Testing</a></li>        
    </ul> 

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
		this.contextMenuSetting = {
                    enable: true,
                    customMenuItems: [
                              { text: "Hide Column", template: "#template" },
                    ]
        };
	}
    
{% endhighlight %}


### columns `Array`
{:#members:columns}

Gets or sets an object that indicates to render the Kanban with specified columns.

#### Default Value:

* Array

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	}
    
{% endhighlight %}


### columns.headerText `string`
{:#members:columns-headertext}

Gets or sets an object that indicates to render the Kanban with specified columns header text.

#### Default Value

* null

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	}
    
{% endhighlight %}


### columns.totalCount `Object`
{:#members:columns-totalcount}

To customize the totalCount properties.
    
#### Default Value:

* Object

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id"  [enableTotalCount]="true">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	}
    
{% endhighlight %}


### columns.totalCount.text `string`
{:#members:columns-totalcount-text}

To customize the totalCount text properties.
    
#### Default Value:

* null

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id"  [enableTotalCount]="true">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog" [totalCount]="totalCount"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	    this.totalCount = { text: "Backlog Count" };
	}
    
{% endhighlight %}


### columns.key `string/number`
{:#members:columns-key}

Gets or sets an object that indicates to render the Kanban with specified columns key.

#### Default Value

* null

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	}
    
{% endhighlight %}


### columns.allowDrop `boolean`
{:#members:columns-allowdrop}

To enable/disable allowDrop for specific column wise.

#### Default Value

* true

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" [allowTitle]="true" keyField="Status" fields.content="Summary" fields.primaryKey="Id" [workflows]="workflow">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog" [allowDrop]="false"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	    this.workflow = [
          { key: "Open", allowedTransitions: "InProgress" },
          { key: "InProgress", allowedTransitions: "Testing,Close" }
        ];
	}
    
{% endhighlight %}


### columns.allowDrag `boolean`
{:#members:columns-allowdrag}

To enable/disable allowDrag for specific column wise.

#### Default Value

* true

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" [allowTitle]="true" keyField="Status" fields.content="Summary" fields.primaryKey="Id" [workflows]="workflow">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done" [allowDrag]="false"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	    this.workflow = [
          { key: "Open", allowedTransitions: "InProgress" },
          { key: "InProgress", allowedTransitions: "Testing,Close" }
        ];
	}
    
{% endhighlight %}


### columns.isCollapsed `boolean`
{:#members:columns-iscollapsed}

To set column collapse or expand state

#### Default Value

* false

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id" [allowToggleColumn]="true">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog" [isCollapsed]="true"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done" allowDrag="false"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	}
    
{% endhighlight %}


### columns.constraints `Object`
{:#members:columns-constraints}

To customize the column level constraints with minimum ,maximum limit validation.

#### Default Value

* Object

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog" [constraints]="constraint"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done" allowDrag="false"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	}
    constraint = { min: 1, max: 2 };
	
{% endhighlight %}

 
### columns.constraints.type `string`
{:#members:columns-constraints-type}

It is used to specify the type of constraints as column or swimlane.

#### Default Value

* null

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress" [constraints]="constraint1"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing" [constraints]="constraint2"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done" allowDrag="false"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	}
    constraint1 = { type: ej.Kanban.Type.Swimlane, min: 1, max: 2 };
	constraint2 = { type: ej.Kanban.Type.Column, max: 2 };
		
{% endhighlight %}

 
### columns.constraints.min `number`
{:#members:columns-constraints-min}

It is used to specify the minimum amount of card in particular column cell or swimlane cell can hold.

#### Default Value

* null

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress" [constraints]="constraint1"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing" [constraints]="constraint2"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done" allowDrag="false"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	}
    constraint1 = { type: ej.Kanban.Type.Swimlane, min: 1, max: 2  };
	constraint2 = { type: ej.Kanban.Type.Column, max: 2 };
	
{% endhighlight %}


### columns.constraints.max `number`
{:#members:columns-constraints-max}

It is used to specify the maximum amount of card in particular column cell or swimlane cell can hold.

#### Default Value

* null

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress" [constraints]="constraint1"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing" [constraints]="constraint2"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done" allowDrag="false"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	}
    constraint1 = { type: ej.Kanban.Type.Swimlane, min: 1, max: 2  };
	constraint2 = { type: ej.Kanban.Type.Column, max: 2 };
{% endhighlight %}

 
### columns.headerTemplate `string`
{:#members:columns-headertemplate}

Gets or sets a value that indicates to add the template within the header element.

#### Default Value

* null

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog" headerTemplate="#column1"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done" headerTemplate="#column4"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>
    <div id="column1">
        <span class="e-backlog e-icon"></span> Backlog
    </div>
    <div id="column4">
        <span class="e-done e-icon"></span> Done
    </div>
    <style>
        .e-backlog,.e-done {
            font-size: 16px;
            padding-right: 5px;
            display: inline-block;
        }    
        .e-backlog:before {
            content: "\e807";
        }    
        .e-done:before {
            content: "\e80a";
        }
    </style>
{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	}
    
{% endhighlight %}

 
### columns.width `string/number`
{:#members:columns-width}

Gets or sets an object that indicates to render the Kanban with specified columns width.

#### Default Value:

* null

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog" width="200"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress" width="200"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing" width="200"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done" width="200"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	}
    
{% endhighlight %}


### columns.visible `boolean`
{:#members:columns-visible}

Gets or sets an object that indicates to set specific column visibility.

#### Default Value:

* true

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing" [visible]="false"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	}
    
{% endhighlight %}


### columns.showAddButton `boolean`
{:#members:columns-showaddbutton}

Gets or sets an object that indicates whether to show add new button.

#### Default Value:

* false

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id" [editSettings.editItems]="editItem" editSettings.allowEditing="true" editSettings.allowAdding="true">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog" showAddButton="true"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	    this.editItem = [
            { field: "Id", editType: ej.Kanban.EditingType.String, validationRules: { required: true, number: true } },
            { field: "Status", editType: ej.Kanban.EditingType.Dropdown },
            { field: "Assignee", editType: ej.Kanban.EditingType.Dropdown },
            { field: "Estimate", editType: ej.Kanban.EditingType.Numeric, editParams: { decimalPlaces: 2 }, validationRules: { range: [0, 1000] } },
            { field: "Summary", editType: ej.Kanban.EditingType.TextArea, validationRules: { required: true } }
        ];
	}
    
{% endhighlight %}

 
### cardSettings `Object`
{:#members:cardsettings}

Gets or sets an object that indicates whether to Customize the card settings.

#### Default Value

* Object

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.color="Type" fields.content="Summary" fields.primaryKey="Id" [cardSettings.colorMapping]="color">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	}
	color = {
        "#cb2027": "Issue,Story",
        "#67ab47": "Improvement",
        "#fbae19": "Epic",
        "#6a5da8": "UG"
    };
    
{% endhighlight %}


### cardSettings.template `string`
{:#members:cardsettings-template}

Gets or sets a value that indicates to add the template for card .

#### Default Value:

* null

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.color="Type" fields.content="Summary" fields.primaryKey="Id" cardSettings.template="#template">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>
	<script id="template" type="text/ng-template">
    <table>
        <tr>
            <td class="photo">
                <img src="../themes/images/kanban/{% raw %}{{:Priority}}{% endraw %}.png">
            </td>
            <td class="details">
                <table>
                    <colgroup>
                        <col width="30%">
                        <col width="70%">
                    </colgroup>
                    <tbody>
                        <tr>
                            <td class="CardHeader">Name: </td>
                            <td>{% raw %}{{:Assignee}}{% endraw %}</td>
                        </tr>
                        <tr>
                            <td class="CardHeader">Task: </td>
                            <td>{% raw %}{{:Type}}{% endraw %}</td>
                        </tr>
                    </tbody>
                </table>
            </td>
        </tr>
    </table>
    </script>
    <style type="text/css">
        .details > table {
            margin-left: 10px;
            border-collapse: separate;
            border-spacing: 7px;
            width: 100%;
        }
        .photo {
            padding-left: 6px;
        }
        .CardHeader {
            font-weight: bolder;
        }
    </style>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	}
    
{% endhighlight %}

       
### cardSettings.colorMapping `Object`
{:#members:cardsettings-colormapping}

To customize the card border color based on assigned task. Colors and corresponding values defined here will be mapped with colorField mapped data source column.

#### Default Value

* Object

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.color="Type" fields.content="Summary" fields.primaryKey="Id" [cardSettings.colorMapping]="color">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	}
	color = {
        "#cb2027": "Issue,Story",
        "#67ab47": "Improvement",
        "#fbae19": "Epic",
        "#6a5da8": "UG"
    };
    
{% endhighlight %}


### customToolbarItems `Array`
{:#members:customtoolbaritems}

Gets or sets a value that indicates whether to add customToolbarItems within the toolbar to perform any action in the Kanban.

#### Default Value:

* []

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id" [customToolbarItems]="customToolbarItems" (toolbarClick)="onToolBarClick($event)" editSettings.allowEditing="true" editSettings.allowAdding="true">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>
	<script id="Delete" type="text/x-jsrender">
        <a class="e-customdelete  e-icon" />
    </script>
    <style type="text/css" class="cssStyles">
        .e-customdelete:before {
            content: "\e800";
            line-height: 26px;
            min-height: 26px;
            min-width: 14px;
            display: inline-block;
        }
    </style>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	    this.customToolbarItems= [{ template: "#Delete" }];
	}
	onToolBarClick(event){
            if (event.itemName == "Delete") {
                        let kObj = $("#kanban").data("ejKanban");
                        let selected = kObj.element.find(".e-cardselection");
                        kObj.KanbanEdit.deleteCard(selected.attr("id"));
            }
    };
    
{% endhighlight %}


### customToolbarItems.template `string`
{:#members:customtoolbaritems-template}

Gets the template to render customToolbarItems.

#### Default Value:
{:.param}
* null

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id" [customToolbarItems]="customToolbarItems" (toolbarClick)="onToolBarClick($event)" editSettings.allowEditing="true" editSettings.allowAdding="true">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>
	<script id="Delete" type="text/x-jsrender">
        <a class="e-customdelete  e-icon" />
    </script>
    <style type="text/css" class="cssStyles">
        .e-customdelete:before {
            content: "\e800";
            line-height: 26px;
            min-height: 26px;
            min-width: 14px;
            display: inline-block;
        }
    </style>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	}
	onToolBarClick(event){
            if (event.itemName == "Delete") {
                        let kObj = $("#kanban").data("ejKanban");
                        let selected = kObj.element.find(".e-cardselection");
                        kObj.KanbanEdit.deleteCard(selected.attr("id"));
            }
    };
    
{% endhighlight %}


### cssClass `string`
{:#members:cssclass}

Gets or sets a value that indicates to render the Kanban with custom theme.

#### Default Value:

* ""

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id" cssClass="gradient-green">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>
	<style type="text/css">
        .gradient-green {
            font-family: cursive;
        }
        .gradient-green .e-swimlanerow {
            background: none repeat scroll 0 0 #71A409;
        }
    </style>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	}
    
{% endhighlight %}

 
### dataSource `Object`
{:#members:datasource}

Gets or sets the data to render the Kanban with cards.

#### Default Value:

* null
 
#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	}
    
{% endhighlight %}


### enableTouch `boolean`
{:#members:enabletouch}

To perform kanban functionalities with touch interaction.

#### Default Value:

* true

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id" enableTouch="false">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	}
    
{% endhighlight %}


### enableRTL `boolean`
{:#members:enablertl}

Align content in the Kanban control align from right to left by setting the property as true.

#### Default Value:

* false

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id" enableRTL="true">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	}
    
{% endhighlight %}


### enableTotalCount `boolean`
{:#members:enabletotalcount}

To show total count of cards in each column. 
    
#### Default Value:

* false

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id" enableTotalCount="true">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	}
    
{% endhighlight %}


### editSettings `Object`
{:#members:editsettings}

Get or sets an object that indicates whether to customize the editing behavior of the Kanban.

#### Default Value:

* Object

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" actionComplete="complete" keyField="Status" fields.content="Summary" fields.primaryKey="Id" [editSettings.editItems]="editItem" editSettings.allowEditing="true" editSettings.allowAdding="true">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	    this.editItem = [
            { field: "Id", editType: ej.Kanban.EditingType.String },
            { field: "Status", editType: ej.Kanban.EditingType.Dropdown },
            { field: "Assignee", editType: ej.Kanban.EditingType.Dropdown },
            { field: "Estimate", editType: ej.Kanban.EditingType.Numeric, editParams: { decimalPlaces: 2 } },
            { field: "Summary", editType: ej.Kanban.EditingType.TextArea }
            ],
        ];
	}
    
{% endhighlight %}


### editSettings.allowEditing `boolean`
{:#members:editsettings-allowediting}

Gets or sets a value that indicates whether to enable the editing action in cards of Kanban.

#### Default Value:

* false

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" actionComplete="complete" keyField="Status" fields.content="Summary" fields.primaryKey="Id" [editSettings.editItems]="editItem" editSettings.allowEditing="true">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	    this.editItem = [
            { field: "Id", editType: ej.Kanban.EditingType.String },
            { field: "Status", editType: ej.Kanban.EditingType.Dropdown },
            { field: "Assignee", editType: ej.Kanban.EditingType.Dropdown },
            { field: "Estimate", editType: ej.Kanban.EditingType.Numeric, editParams: { decimalPlaces: 2 } },
            { field: "Summary", editType: ej.Kanban.EditingType.TextArea }
            ],
        ];
	}
    
{% endhighlight %}


### editSettings.allowAdding `boolean`
{:#members:editsettings-allowadding}

Gets or sets a value that indicates whether to enable the adding action in cards behavior on Kanban.

#### Default Value:

* false

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" actionComplete="complete" keyField="Status" fields.content="Summary" fields.primaryKey="Id" [editSettings.editItems]="editItem" editSettings.allowAdding="true">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	    this.editItem = [
            { field: "Id", editType: ej.Kanban.EditingType.String },
            { field: "Status", editType: ej.Kanban.EditingType.Dropdown },
            { field: "Assignee", editType: ej.Kanban.EditingType.Dropdown },
            { field: "Estimate", editType: ej.Kanban.EditingType.Numeric, editParams: { decimalPlaces: 2 } },
            { field: "Summary", editType: ej.Kanban.EditingType.TextArea }
            ],
        ];
	}
    
{% endhighlight %}


### editSettings.dialogTemplate `string`
{:#members:editsettings-dialogtemplate}

This specifies the id of the template which is require to be edited using the Dialog Box.

#### Default Value:

* null

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id" editSettings.allowEditing="true" editSettings.allowAdding="true" editSettings.editMode="ej.Kanban.EditMode.DialogTemplate" editSettings.dialogTemplate="#template">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>
	<script id="template" type="text/template">
    <table>
        <tr>
            <td style="text-align: right;">Id
            </td>
            <td style="text-align: left">
                <input id="Id" name="Id" value="" class="e-field e-ejinputtext valid e-disable" disabled="disabled" />
            </td>
            <td style="text-align: right;">Status
            </td>
            <td style="text-align: left">
                <input id="Status" name="Status" value="" class="e-field e-ejinputtext valid" />
            </td>
        </tr>
    </table>
    </script> <script id="template" type="text/template">
    <table>
        <tr>
            <td style="text-align: right;">Id
            </td>
            <td style="text-align: left">
                <input id="Id" name="Id" value="" class="e-field e-ejinputtext valid e-disable" disabled="disabled" />
            </td>
            <td style="text-align: right;">Status
            </td>
            <td style="text-align: left">
                <input id="Status" name="Status" value="" class="e-field e-ejinputtext valid" />
            </td>
        </tr>
    </table>
    </script>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	}
    
{% endhighlight %}


### editSettings.editMode `enum`
{:#members:editsettings-editmode}

<ts name="ej.Kanban.EditMode"/>

Get or sets an object that indicates whether to customize the editMode of the Kanban.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">Dialog</td>
<td class="description">Creates Kanban with editMode as Dialog</td>
</tr>
<tr>
<td class="name">DialogTemplate</td>
<td class="description">Creates Kanban with editMode as DialogTemplate</td>
</tr>
<tr>
<td class="name">ExternalForm</td>
<td class="description">Creates Kanban with editMode as ExternalForm</td>
</tr>
<tr>
<td class="name">ExternalFormTemplate</td>
<td class="description">Creates Kanban with editMode as ExternalFormTemplate</td>
</tr>
</tbody>
</table>

#### Default Value:

* ej.Kanban.EditMode.Dialog

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id" editSettings.editMode="ej.Kanban.EditMode.Dialog" [editSettings.editItems]="editItem" editSettings.allowEditing="true" editSettings.allowAdding="true">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	    this.editItem = [
            { field: "Id", editType: ej.Kanban.EditingType.String },
            { field: "Status", editType: ej.Kanban.EditingType.Dropdown },
            { field: "Assignee", editType: ej.Kanban.EditingType.Dropdown },
            { field: "Estimate", editType: ej.Kanban.EditingType.Numeric, editParams: { decimalPlaces: 2 } },
            { field: "Summary", editType: ej.Kanban.EditingType.TextArea }
        ];
	}
    
{% endhighlight %}


### editSettings.editItems `Array`
{:#members: editsettings-edititems}

Get or sets an object that indicates whether to customize the editing fields of Kanban card.

#### Default Value:

* Array

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id" editSettings.editMode="ej.Kanban.EditMode.Dialog" [editSettings.editItems]="editItem" editSettings.allowEditing="true" editSettings.allowAdding="true">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	    this.editItem = [
            { field: "Id", editType: ej.Kanban.EditingType.String },
            { field: "Status", editType: ej.Kanban.EditingType.Dropdown },
            { field: "Assignee", editType: ej.Kanban.EditingType.Dropdown },
            { field: "Estimate", editType: ej.Kanban.EditingType.Numeric, editParams: { decimalPlaces: 2 } },
            { field: "Summary", editType: ej.Kanban.EditingType.TextArea }
        ];
	}
    
{% endhighlight %}


### editSettings.editItems.field `string`
{:#members:editsettings-edititems-field}

It is used to map editing field from the data source.

#### Default Value:

* null

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id" editSettings.editMode="ej.Kanban.EditMode.Dialog" [editSettings.editItems]="editItem" editSettings.allowEditing="true" editSettings.allowAdding="true">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	    this.editItem = [
            { field: "Id", editType: ej.Kanban.EditingType.String },
            { field: "Status", editType: ej.Kanban.EditingType.Dropdown },
            { field: "Assignee", editType: ej.Kanban.EditingType.Dropdown },
            { field: "Estimate", editType: ej.Kanban.EditingType.Numeric, editParams: { decimalPlaces: 2 } },
            { field: "Summary", editType: ej.Kanban.EditingType.TextArea }
        ];
	}
    
{% endhighlight %}


### editSettings.editItems.editType `enum`
{:#members:editsettings-edititems-edittype}

<ts name="ej.Kanban.EditingType"/>

It is used to set the particular editType in the card for editing.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">String</td>
<td class="description">Allows to set edit type as string edit type</td>
</tr>
<tr>
<td class="name">Numeric</td>
<td class="description">Allows to set edit type as numeric edit type </td>
</tr>
<tr>
<td class="name">Dropdown</td>
<td class="description">Allows to set edit type as drop down edit type</td>
</tr>
<tr>
<td class="name">DatePicker</td>
<td class="description">Allows to set edit type as date picker edit type</td>
</tr>
<tr>
<td class="name">DateTimePicker</td>
<td class="description">Allows to set edit type as date time picker edit type</td>
</tr>
<tr>
<td class="name">TextArea</td>
<td class="description">Allows to set edit type as text area edit type</td>
</tr>
<tr>
<td class="name">RTE</td>
<td class="description">Allows to set edit type as RTE edit type</td>
</tr>
</tbody>
</table>

#### Default Value:

* ej.Kanban.EditingType.String

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id" editSettings.editMode="ej.Kanban.EditMode.Dialog" [editSettings.editItems]="editItem" editSettings.allowEditing="true" editSettings.allowAdding="true">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	    this.editItem = [
            { field: "Id", editType: ej.Kanban.EditingType.String },
            { field: "Status", editType: ej.Kanban.EditingType.Dropdown },
            { field: "Assignee", editType: ej.Kanban.EditingType.Dropdown },
            { field: "Estimate", editType: ej.Kanban.EditingType.Numeric, editParams: { decimalPlaces: 2 } },
            { field: "Summary", editType: ej.Kanban.EditingType.TextArea }
        ];
	}
    
{% endhighlight %}


### editSettings.editItems.validationRules `Object`
{:#members:editsettings-edititems-validationrules}

Gets or sets a value that indicates to define constraints for saving data to the database.

#### Default Value

* Object

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id" editSettings.editMode="ej.Kanban.EditMode.Dialog" [editSettings.editItems]="editItem" editSettings.allowEditing="true" editSettings.allowAdding="true">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	    this.editItem = [
            { field: "Id", editType: ej.Kanban.EditingType.String, validationRules: { required: true, number: true } },
            { field: "Status", editType: ej.Kanban.EditingType.Dropdown },
            { field: "Assignee", editType: ej.Kanban.EditingType.Dropdown },
            { field: "Estimate", editType: ej.Kanban.EditingType.Numeric, editParams: { decimalPlaces: 2 }, validationRules: { range: [0, 1000] } },
            { field: "Summary", editType: ej.Kanban.EditingType.TextArea, validationRules: { required: true } }
        ];
	}
    
{% endhighlight %}


### editSettings.editItems.editParams `Object`
{:#members:editsettings-edititems-editparams}

It is used to set the particular editParams in the card for editing.

#### Default Value:

* Object

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id" editSettings.editMode="ej.Kanban.EditMode.Dialog" [editSettings.editItems]="editItem" editSettings.allowEditing="true" editSettings.allowAdding="true">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	    this.editItem = [
            { field: "Id", editType: ej.Kanban.EditingType.String },
            { field: "Status", editType: ej.Kanban.EditingType.Dropdown },
            { field: "Assignee", editType: ej.Kanban.EditingType.Dropdown },
            { field: "Estimate", editType: ej.Kanban.EditingType.Numeric, editParams: { decimalPlaces: 2 } },
            { field: "Summary", editType: ej.Kanban.EditingType.TextArea }
        ];
	}
    
{% endhighlight %}


### editSettings.editItems.defaultValue `string/number`
{:#members:editsettings-edititems-defaultvalue}

It is used to specify defaultValue for the fields while adding new card.

#### Default Value

* null

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id" editSettings.editMode="ej.Kanban.EditMode.Dialog" [editSettings.editItems]="editItem" editSettings.allowEditing="true" editSettings.allowAdding="true">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	    this.editItem = [
            { field: "Id", editType: ej.Kanban.EditingType.String, validationRules: { required: true, number: true } },
            { field: "Status", editType: ej.Kanban.EditingType.String, defaultValue: "Open" },
            { field: "Assignee", editType: ej.Kanban.EditingType.Dropdown },
            { field: "Estimate", editType: ej.Kanban.EditingType.Numeric, editParams: { decimalPlaces: 2 }, validationRules: { range: [0, 1000] } },
            { field: "Summary", editType: ej.Kanban.EditingType.TextArea, validationRules: { required: true } }
        ];
	}
    
{% endhighlight %}


### editSettings.externalFormTemplate `string`
{:#members:editsettings-externalformtemplate}

This specifies the id of the template which is require to be edited using the External edit form.

#### Default Value:
{:.param}
* null

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id" editSettings.allowEditing="true" editSettings.allowAdding="true" editSettings.editMode="ej.Kanban.EditMode.ExternalFormTemplate" [editSettings.externalFormTemplate]="#template">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>
	<script id="template" type="text/template">
    <table>
        <tr>
            <td style="text-align: right;">Id
            </td>
            <td style="text-align: left">
                <input id="Id" name="Id" value="" class="e-field e-ejinputtext valid e-disable" disabled="disabled" />
            </td>
            <td style="text-align: right;">Status
            </td>
            <td style="text-align: left">
                <input id="Status" name="Status" value="" class="e-field e-ejinputtext valid" />
            </td>
        </tr>
    </table>
    </script>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	}
    
{% endhighlight %}


### editSettings.formPosition `enum`
{:#members:editsettings-formposition}

<ts name="ej.Kanban.FormPosition"/>

This specifies to set the position of an External edit form either in the right or bottom of the Kanban.

#### Default Value:

* ej.Kanban.FormPosition.Bottom

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">Bottom</td>
<td class="description">Form position is bottom.</td>
</tr>
<tr>
<td class="name">Right</td>
<td class="description">Form position is right.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id" editSettings.editMode="ej.Kanban.EditMode.ExternalForm" [editSettings.formPosition]="ej.Kanban.FormPosition.Bottom" [editSettings.editItems]="editItem" editSettings.allowEditing="true" editSettings.allowAdding="true">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	    this.editItem = [
            { field: "Id", editType: ej.Kanban.EditingType.String },
            { field: "Status", editType: ej.Kanban.EditingType.String },
            { field: "Assignee", editType: ej.Kanban.EditingType.Dropdown },
            { field: "Estimate", editType: ej.Kanban.EditingType.Numeric, editParams: { decimalPlaces: 2 } },
            { field: "Summary", editType: ej.Kanban.EditingType.TextArea }
        ];
	}
    
{% endhighlight %}

            
### fields `Object`
{:#members:fields}

To customize field mappings for card , editing title and control key parameters

#### Default Value:

* Object

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id" fields.swimlaneKey="Assignee" fields.tag="Tags" fields.title="Id" fields.color="Type" fields.imageUrl="ImgUrl" [cardSettings.colorMapping]="color">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

   constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	}
    color = {
        "#cb2027": "Issue,Story",
        "#67ab47": "Improvement",
        "#fbae19": "Epic",
        "#6a5da8": "UG"
    };
	
{% endhighlight %}


### fields.primaryKey `string`
{:#members:fields-primarykey}

The primaryKey field is mapped to data source field. And this will used for Drag and drop and editing mainly.

#### Default Value:

* null

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	}
	
{% endhighlight %}


### fields.swimlaneKey `string`
{:#members:fields-swimlanekey}

To enable swimlane grouping based on the given key field from datasource mapping.

#### Default Value

* null

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id" fields.swimlaneKey="Assignee">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	}
	
{% endhighlight %}


### fields.priority `string`
{:#members:fields-priority}

Priority field has been mapped data source field to maintain cards priority.

#### Default Value:

* null

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id" fields.priority="RankId">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	}
	
{% endhighlight %}


### fields.content `string`
{:#members:fields-content}

Content field has been Mapped into card text.

#### Default Value:

* null

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	}
	
{% endhighlight %}


### fields.tag `string`
{:#members:fields-tag}

Tag field has been Mapped into card tag.

#### Default Value:

* null

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id" fields.tag="Tags">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	}
	
{% endhighlight %}


### fields.title `string`
{:#members:fields-title}

Title field has been Mapped to field in datasource for title content. If title field specified , card expand/collapse will be enabled with header and content section.

#### Default Value:

* null

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id" fields.title="Assignee">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	}
	
{% endhighlight %}


### fields.color `string`
{:#members:fields-color}

To customize the card has been Mapped into card color field.

#### Default Value:

* null

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id" fields.color="Type" [cardSettings.colorMapping]="color">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

   constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	}
    color = {
        "#cb2027": "Issue,Story",
        "#67ab47": "Improvement",
        "#fbae19": "Epic",
        "#6a5da8": "UG"
    };
	
{% endhighlight %}


### fields.imageUrl `string`
{:#members:fields-imageurl}

ImageUrl field has been Mapped into card image.

#### Default Value

* null

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id" fields.imageUrl="ImgUrl">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	}
	
{% endhighlight %}


### fields.collapsibleCards `Object`
{:#members:fields-collapsiblecards}

Get or sets an object that indicates the options to map the cards to the collapsible area.

#### Default Value

* Object

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id" [fields.collapsibleCards]="collapsibleCards">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

   constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	    this.collapsibleCards = { field: "Status", key: "Close" };
	}
	
{% endhighlight %}


### fields.collapsibleCards.field `string`
{:#members:fields-collapsiblecards-field}

It is used to specify the collapsible card's field mapping.

#### Default Value

* null

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id" [fields.collapsibleCards]="collapsibleCards">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

   constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	    this.collapsibleCards = { field: "Status", key: "Close" };
	}
	
{% endhighlight %}


### fields.collapsibleCards.key `string`
{:#members:fields-collapsiblecards-key}

It is used to specify the collapsible card's key mapping which is available in datasource value of field mapped in `collapsibleCards.field`.

#### Default Value

* null

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id" [fields.collapsibleCards]="collapsibleCards">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

   constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	    this.collapsibleCards = { field: "Status", key: "Close" };
	}
	
{% endhighlight %}


### keyField `string`
{:#members:keyfield}

To map datasource field for column values mapping 

#### Default Value:

* null

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

   constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	}
	
{% endhighlight %}


### isResponsive `boolean`
{:#members:isresponsive}

When set to true, adapts the Kanban layout to fit the screen size of devices on which it renders.

#### Default Value:

* false

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id" isResponsive="true">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

   constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	}
	
{% endhighlight %}


### minWidth `number`
{:#members:minwidth}

Gets or sets a value that indicates whether to set the minimum width of the responsive Kanban while isResponsive property is true.

#### Default Value:

* 0

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" minWidth="400" keyField="Status" fields.content="Summary" fields.primaryKey="Id" isResponsive="true">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog" width="150"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress" width="120"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing" width="120"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done" width="150"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

   constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	}
	
{% endhighlight %}


### filterSettings `Array`
{:#members:filtersettings}

To customize the filtering behavior based on queries given.

#### Default Value:

* Array

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" allowFiltering="true" keyField="Status" fields.content="Summary" fields.primaryKey="Id" [filterSettings]="filterSetting">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

   constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	    this.filterSetting = [
            { text: "Janet Issues", query: new ej.Query().where("Assignee", "equal", "Janet Leverling"), description: "Displays issues which matches the assignee as 'Janet Leverling'" },
            { text: "Closed Issues", query: new ej.Query().where("Status", "equal", "Close"), description: "Display the 'Closed' issues" }
        ];
	}
	
{% endhighlight %}


### filterSettings.text `string`
{:#members:filtersettings-text}

Gets or sets an object of display name to filter queries.

#### Default Value:

* null

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" allowFiltering="true" keyField="Status" fields.content="Summary" fields.primaryKey="Id" [filterSettings]="filterSetting">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

   constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	    this.filterSetting = [
            { text: "Janet Issues", query: new ej.Query().where("Assignee", "equal", "Janet Leverling"), description: "Displays issues which matches the assignee as 'Janet Leverling'" },
            { text: "Closed Issues", query: new ej.Query().where("Status", "equal", "Close"), description: "Display the 'Closed' issues" }
        ];
	}
	
{% endhighlight %}


### filterSettings.query `Object`
{:#members:filtersettings-query}

Gets or sets an object that Queries to perform filtering

#### Default Value:

* Object

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" allowFiltering="true" keyField="Status" fields.content="Summary" fields.primaryKey="Id" [filterSettings]="filterSetting">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

   constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	    this.filterSetting = [
            { text: "Janet Issues", query: new ej.Query().where("Assignee", "equal", "Janet Leverling"), description: "Displays issues which matches the assignee as 'Janet Leverling'" },
            { text: "Closed Issues", query: new ej.Query().where("Status", "equal", "Close"), description: "Display the 'Closed' issues" }
        ];
	}
	
{% endhighlight %}


### filterSettings.description `string`
{:#members:filtersettings-description}

Gets or sets an object of tooltip to filter buttons.

#### Default Value:

* null

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" allowFiltering="true" keyField="Status" fields.content="Summary" fields.primaryKey="Id" [filterSettings]="filterSetting">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

   constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	    this.filterSetting = [
            { text: "Janet Issues", query: new ej.Query().where("Assignee", "equal", "Janet Leverling"), description: "Displays issues which matches the assignee as 'Janet Leverling'" },
            { text: "Closed Issues", query: new ej.Query().where("Status", "equal", "Close"), description: "Display the 'Closed' issues" }
        ];
	}
	
{% endhighlight %}


### query `Object`
{:#members:query}

ej Query to query database of Kanban.

#### Default Value:

* null

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id" [query]="query">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	    this.query = ej.Query().select(["Status", "Id", "Summary"]);
	}
	
{% endhighlight %}


### keySettings `Object`
{:#members:keysettings}

To change the key in keyboard interaction to Kanban control.

#### Default Value

* null

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" allowKeyboardNavigation="true" selectionType="multiple" [keySettings]="keySettings" keyField="Status" fields.content="Summary" fields.primaryKey="Id" [editSettings.editItems]="editItem" editSettings.allowEditing="true" editSettings.allowAdding="true">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	    this.editItem = [
            { field: 'Id' },
            { field: 'Status', editType: ej.Kanban.EditingType.Dropdown },
            { field: 'Assignee', editType: ej.Kanban.EditingType.Dropdown },
            { field: 'Estimate', editType: ej.Kanban.EditingType.Numeric, editParams: { decimalPlaces: 2 } },
            { field: 'Summary', editType: ej.Kanban.EditingType.TextArea, editParams: { height: 100, width: 200 } }
        ];
		this.keySettings={focus: "e",insertCard: "45"};
	}
	
{% endhighlight %}


### scrollSettings `Object`
{:#members:scrollsettings}

Gets or sets an object that indicates whether to customize the scrolling behavior of the Kanban.

#### Default Value:

* Object

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" allowScrolling="true" keyField="Status" fields.content="Summary" fields.primaryKey="Id" fields.swimlaneKey="Assignee" [scrollSettings]="scrollSetting">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

	constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	    this.scrollSetting = {width:700,height:400};
	}
    
{% endhighlight %}


### scrollSettings.height `string/number`
{:#members:scrollsettings-height}

Gets or sets an object that indicates to render the Kanban with specified scroll height.

#### Default Value:

* 0

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" allowScrolling="true" keyField="Status" fields.content="Summary" fields.primaryKey="Id" fields.swimlaneKey="Assignee" [scrollSettings]="scrollSetting">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	    this.scrollSetting = {height:400};
	}
    
{% endhighlight %}


### scrollSettings.width `string/number`
{:#members:scrollsettings-width}

Gets or sets an object that indicates to render the Kanban with specified scroll width.

#### Default Value:

* auto

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" allowScrolling="true" keyField="Status" fields.content="Summary" fields.primaryKey="Id" fields.swimlaneKey="Assignee" [scrollSettings]="scrollSetting">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

	constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	    this.scrollSetting = {width:700,height:400};
	}
    
{% endhighlight %}


### scrollSettings.allowFreezeSwimlane `boolean`
{:#members:scrollsettings-allowfreezeswimlane}

To allow the Kanban to freeze particular swimlane at the time of scrolling , until scroll reaches next swimlane and it continues.

#### Default Value:

* false

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" allowScrolling="true" keyField="Status" fields.content="Summary" fields.primaryKey="Id" fields.swimlaneKey="Assignee" [scrollSettings]="scrollSetting">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog" width="250"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress" width="220"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing" width="220"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done" width="250"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

	constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	    this.scrollSetting = {width:800,height:500,allowFreezeSwimlane:true};
	}
    
{% endhighlight %}


### searchSettings `Object`
{:#members:searchsettings}

To customize the searching behavior of the Kanban.

#### Default Value:

* Object

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" allowSearching="true" keyField="Status" fields.content="Summary" fields.primaryKey="Id" [searchSettings]="searchSetting">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog" width="250"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress" width="220"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing" width="220"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done" width="250"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

	constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	    this.searchSetting = {fields: ["Summary", "Id"],key: "",operator: "contains",ignoreCase: true};
	}
    
{% endhighlight %}


### searchSettings.fields `Array`
{:#members:searchsettings-fields}

To customize the fields the searching operation can be perform.

#### Default Value:

* Array

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" allowSearching="true" keyField="Status" fields.content="Summary" fields.primaryKey="Id" [searchSettings]="searchSetting">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog" width="250"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress" width="220"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing" width="220"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done" width="250"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

	constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	    this.searchSetting = {fields: ["Summary", "Id"],key: "",operator: "contains",ignoreCase: true};
	}
    
{% endhighlight %}


### searchSettings.key `string`
{:#members:searchsettings-key}

To customize the searching string.

#### Default Value:

* ""

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" allowSearching="true" keyField="Status" fields.content="Summary" fields.primaryKey="Id" [searchSettings]="searchSetting">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog" width="250"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress" width="220"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing" width="220"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done" width="250"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

	constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	    this.searchSetting = {key: "Analyze",operator: "contains",ignoreCase: true};
	}
    
{% endhighlight %}


### searchSettings.operator `string`
{:#members:searchsettings-operator}

To customize the operator based on searching.

#### Default Value:

* contains

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" allowSearching="true" keyField="Status" fields.content="Summary" fields.primaryKey="Id" [searchSettings]="searchSetting">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog" width="250"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress" width="220"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing" width="220"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done" width="250"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

	constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	    this.searchSetting = {key: "Analyze",operator: "contains",ignoreCase: true};
	}
    
{% endhighlight %}


### searchSettings.ignoreCase `boolean`
{:#members:searchsettings-ignorecase}

To customize the ignore case based on searching.

#### Default Value:

* true

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" allowSearching="true" keyField="Status" fields.content="Summary" fields.primaryKey="Id" [searchSettings]="searchSetting">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog" width="250"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress" width="220"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing" width="220"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done" width="250"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

	constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	    this.searchSetting = {key: "analyze",operator: "contains",ignoreCase: true};
	}
    
{% endhighlight %}


### selectionType `enum`
{:#members:selectiontype}

<ts name="ej.Kanban.SelectionType"/>

To allow customize selection type. Accepting types are "single" and "multiple".

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">Single</td>
<td class="description">Support for Single selection in Kanban</td>
</tr>
<tr>
<td class="name">Multiple</td>
<td class="description">Support for multiple selections in Kanban</td>
</tr>
</tbody>
</table>

#### Default Value:

* ej.Kanban.SelectionType.Single

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id" selectionType="multiple">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

   constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	}
	
{% endhighlight %}


### stackedHeaderRows `Array`
{:#members:stackedheaderrows}

Gets or sets an object that indicates to managing the collection of stacked header rows for the Kanban.

#### Default Value:

* Array

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id" [stackedHeaderRows]="stackedHeaderRow">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
		<e-kanban-column key="Validated" headertext="Validated"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

   constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	    this.stackedHeaderRow = [{stackedHeaderColumns: [{ headerText: "Unresolved", column: "Backlog,Validated,In Progress" }, { headerText: "Resolved", column: "Testing,Done" }];
	}
	
{% endhighlight %}


### stackedHeaderRows.stackedHeaderColumns `Array`
{:#members:stackedheaderrows-stackedheadercolumns}

Gets or sets a value that indicates whether to add stacked header columns into the stacked header rows.

#### Default Value:

* Array

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id" [stackedHeaderRows]="stackedHeaderRow">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
		<e-kanban-column key="Validated" headertext="Validated"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

   constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	    this.stackedHeaderRow = [{stackedHeaderColumns: [{ headerText: "Unresolved", column: "Backlog,Validated,In Progress" }, { headerText: "Resolved", column: "Testing,Done" }];
	}
	
{% endhighlight %}


### stackedHeaderRows.stackedHeaderColumns.headerText `string`
{:#members:stackedheaderrows-stackedheadercolumns-headertext}

Gets or sets a value that indicates the headerText for the particular stacked header column.

#### Default Value:

* null

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id" [stackedHeaderRows]="stackedHeaderRow">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
		<e-kanban-column key="Validated" headertext="Validated"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

   constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	    this.stackedHeaderRow = [{stackedHeaderColumns: [{ headerText: "Unresolved", column: "Backlog,Validated,In Progress" }, { headerText: "Resolved", column: "Testing,Done" }];
	}
	
{% endhighlight %}


### stackedHeaderRows.stackedHeaderColumns.column `string`
{:#members:stackedheaderrows-stackedheadercolumns-column}

Gets or sets a value that indicates the column for the particular stacked header column.

#### Default Value

* null

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id" [stackedHeaderRows]="stackedHeaderRow">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
		<e-kanban-column key="Validated" headertext="Validated"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	    this.stackedHeaderRow = [{stackedHeaderColumns: [{ headerText: "Unresolved", column: "Backlog,Validated,In Progress" }, { headerText: "Resolved", column: "Testing,Done" }];
	}
	
{% endhighlight %}


### tooltipSettings `Object`
{:#members:tooltipsettings}

The tooltip allows to display card details in a tooltip while hovering on it.

### tooltipSettings.enable `boolean`
{:#members:tooltipsettings-enable}

To enable or disable the tooltip display.


#### Default Value

* false

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id" fields.swimlaneKey="Assignee" fields.tag="Tags" fields.title="Id" fields.color="Type" fields.imageUrl="ImgUrl" [tooltipSettings.enable]="true" [cardSettings.colorMapping]="color">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	}
	color = {
        "#cb2027": "Issue,Story",
        "#67ab47": "Improvement",
        "#fbae19": "Epic",
        "#6a5da8": "UG"
    };
    
{% endhighlight %}


### tooltipSettings.template `string`
{:#members:tooltipsettings-template}

To customize the tooltip display based on your requirements.

#### Default Value:

* null

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" keyField="Status" fields.content="Summary" fields.primaryKey="Id" fields.swimlaneKey="Assignee" fields.tag="Tags" fields.title="Id" fields.color="Type" fields.imageUrl="ImgUrl" [tooltipSettings]="tooltipSetting" [cardSettings.colorMapping]="color">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>
	<script id="tooltipTemp" type="text/x-jsrender">
    <div class='e-kanbantooltiptemp ' style="display: none">
        <table>
            <tr>
                <td class="photo">
                    <img src="">
                </td>

                <td class="details">
                    <table>
                        <colgroup>
                            <col width="30%">
                            <col width="70%">
                        </colgroup>
                        <tbody>
                            <tr>
                                <td class="CardHeader">Name: </td>
                                <td></td>
                            </tr>
                            <tr>
                                <td class="CardHeader">Task: </td>
                                <td></td>
                            </tr>
                        </tbody>
                    </table>
                </td>
            </tr>
        </table>
    </div>
    </script>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	    this.tooltipSetting={enable: true,template: "#tooltipTemp"};
	}
	color = {
        "#cb2027": "Issue,Story",
        "#67ab47": "Improvement",
        "#fbae19": "Epic",
        "#6a5da8": "UG"
    };
    
{% endhighlight %}

  
### workflows `Array`
{:#members:workflows}

Gets or sets an object that indicates to render the Kanban with specified workflows.

#### Default Value

* Array

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" [allowTitle]="true" [enableTotalCount]="true" allowToggleColumn="true" keyField="Status" fields.content="Summary" fields.primaryKey="Id" [workflows]="workflow">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done" allowDrag="false"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	    this.workflow = [
          { key: "Open", allowedTransitions: "InProgress" },
          { key: "InProgress", allowedTransitions: "Testing,Close" }
        }
	}
    
{% endhighlight %}


### workflows.key  `string/number`
{:#members:workflows-key}

Gets or sets an object that indicates to render the Kanban with specified workflows key.

#### Default Value

* null

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" [allowTitle]="true" [enableTotalCount]="true" allowToggleColumn="true" keyField="Status" fields.content="Summary" fields.primaryKey="Id" [workflows]="workflow">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done" allowDrag="false"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	    this.workflow = [
          { key: "Open", allowedTransitions: "InProgress" },
          { key: "InProgress", allowedTransitions: "Testing,Close" }
        }
	}
    
{% endhighlight %}


### workflows.allowedTransitions `string`
{:#members:workflows-allowedtransitions}

Gets or sets an object that indicates to render the Kanban with specified workflows allowed Transitions.

#### Default Value

* null

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" [allowTitle]="true" [enableTotalCount]="true" allowToggleColumn="true" keyField="Status" fields.content="Summary" fields.primaryKey="Id" [workflows]="workflow">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done" allowDrag="false"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

    constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
	    this.workflow = [
          { key: "Open", allowedTransitions: "InProgress" },
          { key: "InProgress", allowedTransitions: "Testing,Close" }
        }
	}
    
{% endhighlight %}


### locale `string`
{:#members:locale}

Gets or sets a value that indicates whether to customizing the user interface (UI) as locale-specific in order to display regional data i.e. in a language and culture specific to a particular country or region.

#### Default Value:

* "en-US"

#### Example

{% highlight html %}

	<ej-kanban id="kanban" [dataSource]="kanbanData" [allowTitle]="true" keyField="Status" fields.content="Summary" fields.primaryKey="Id" fields.swimlaneKey="Assignee" locale="de-DE">
      <e-kanban-columns>
        <e-kanban-column key="Open" headertext="Backlog"></e-kanban-column>
        <e-kanban-column key="InProgress" headertext="In Progress" constraints.max="2"></e-kanban-column>
		<e-kanban-column key="Testing" headertext="Testing"></e-kanban-column>
        <e-kanban-column key="Close" headertext="Done"></e-kanban-column>
      </e-kanban-columns>
    </ej-kanban>

{% endhighlight %}

{% highlight ts %}

   constructor() {
        this.kanbanData = [{ Id: 1, Status: "Open", Summary: "Analyze the new requirements gathered from the customer.", Type: "Story", Priority: "Low", Tags: "Analyze,Customer", Estimate: 3.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 1 }, { Id: 2, Status: "InProgress", Summary: "Improve application performance", Type: "Improvement", Priority: "Normal", Tags: "Improvement", Estimate: 6, Assignee: "Andrew Fuller", ImgUrl: "/images/kanban/2.png", RankId: 1 }, { Id: 3, Status: "Open", Summary: "Arrange a web meeting with the customer to get new requirements.", Type: "Others", Priority: "Critical", Tags: "Meeting", Estimate: 5.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 4, Status: "InProgress", Summary: "Fix the issues reported in the IE browser.", Type: "Bug", Priority: "Release Breaker", Tags: "IE", Estimate: 2.5, Assignee: "Janet Leverling", ImgUrl: "/images/kanban/3.png", RankId: 2 }, { Id: 5, Status: "Testing", Summary: "Fix the issues reported by the customer.", Type: "Bug", Priority: "Low", Tags: "Customer", Estimate: "3.5", Assignee: "Steven walker", ImgUrl: "/images/kanban/5.png", RankId: 1 }, { Id: 6, Status: "Close", Summary: "Arrange a web meeting with the customer to get the login page requirements.", Type: "Others", Priority: "Low", Tags: "Meeting", Estimate: 2, Assignee: "Michael Suyama", ImgUrl: "/images/kanban/6.png", RankId: 1 }, { Id: 7, Status: "Validate", Summary: "Validate new requirements", Type: "Improvement", Priority: "Low", Tags: "Validation", Estimate: 1.5, Assignee: "Robert King", ImgUrl: "/images/kanban/7.png", RankId: 1 }, { Id: 8, Status: "Close", Summary: "Login page validation", Type: "Story", Priority: "Release Breaker", Tags: "Validation,Fix", Estimate: 2.5, Assignee: "Laura Callahan", ImgUrl: "/images/kanban/8.png", RankId: 2 }, { Id: 9, Status: "Testing", Summary: "Fix the issues reported in Safari browser.", Type: "Bug", Priority: "Release Breaker", Tags: "Fix,Safari", Estimate: 1.5, Assignee: "Nancy Davloio", ImgUrl: "/images/kanban/1.png", RankId: 2 }, { Id: 10, Status: "Close", Summary: "Test the application in the IE browser.", Type: "Story", Priority: "Low", Tags: "Testing,IE", Estimate: 5.5, Assignee: "Margaret hamilt", ImgUrl: "/images/kanban/4.png", RankId: 3 }];
        ej.Kanban.Locale["de-DE"] = {
            EmptyCard: "Keine Karten angezeigt werden",
            SaveButton: "Speichern",
            CancelButton: "stornieren",
            EditFormTitle: "Details von ",
            AddFormTitle: "Neue Karte hinzufügen",
            SwimlaneCaptionFormat: "- 8 Artikel  Artikel ",
            FilterSettings: "Filter:",
            FilterOfText: "Von",
            Max: "Max.",
            Min: "Min.",
            Cards: "Karten",
            ItemsCount: "Artikel Graf :",
            Unassigned: "Nicht zugewiesen",
        };	
	}
	
{% endhighlight %}


## Methods

### columns(column,key,\[action\])
{:#methods:columns}

Add or remove columns in Kanban columns collections.Default action is add.

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
    <td class="name">column details</td>
    <td class="type"><span class="param-type">array/string</span></td>
    <td class="description last">Pass array of columns or string of headerText to add/remove the column in Kanban</td>
    </tr>
    <tr>
    <td class="name">key value</td>
    <td class="type"><span class="param-type">array/string</span></td>
    <td class="description last">Pass array of columns or string of key value to add/remove the column in Kanban</td>
    </tr>
    <tr>
    <td class="name">action</td>
    <td class="type"><span class="param-type">string</span></td>
    <td class="description last"><span class="optional">optional</span> Pass add/remove action to be performed. By default "add" action will perform</td>
    </tr>
    </tbody>
    </table>

#### Example

{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Kanban.widget.columns("Testing","Testing", "remove");   // remove Kanban column
} 
@ViewChild('kanban') Kanban: EJComponents<any, any>;   // Create kanban instance.
}
{% endhighlight %}


### destroy()
{:#methods:destroy}

Destroy the Kanban widget all events bound using this._on will be unbind automatically and bring the control to pre-init state.

#### Example

{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Kanban.widget.destroy();   // destroy the Kanban
} 
@ViewChild('kanban') Kanban: EJComponents<any, any>;   // Create kanban instance.
}
{% endhighlight %}


### dataSource(datasource)
{:#methods:datasource}

Refresh the Kanban with new data source.

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
    <td class="name">datasource</td><td class="type"><span class="param-type">array</span></td>
    <td class="description last">Pass new data source to the Kanban</td>
    </tr>
    </tbody>
    </table>

#### Example

{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Kanban.widget.dataSource(data);   // Refreshes the kanban data source
} 
@ViewChild('kanban') Kanban: EJComponents<any, any>;   // Create kanban instance.
}
{% endhighlight %}


### toggleColumn(headerText or $div)
{:#methods:togglecolumn}

toggleColumn based on the headerText in Kanban.

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
    <td class="name">
    headerText
    </td>
    <td class="type"><span class="param-type">object</span></td>
    <td class="description last">Pass the header text of the column to get the corresponding column object</td>
    </tr>
    </tbody>
    </table>

#### Example

{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Kanban.widget.toggleColumn("Backlog");    // toggleColumn the row based on the row state
} 
@ViewChild('kanban') Kanban: EJComponents<any, any>;   // Create kanban instance.
}
{% endhighlight %}


### toggleCard($div or id)
{:#methods:togglecard}

Expand or collapse the card based on the state of target "div"

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
    <td class="name">
    key
    </td>
    <td class="type"><span class="param-type">string/number</span></td>
    <td class="description last">Pass the id of card to be toggle </td>
    </tr>
    </tbody>
    </table>

#### Example

{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Kanban.widget.toggleCard("2");    // toggleCard the row based on the row state
} 
@ViewChild('kanban') Kanban: EJComponents<any, any>;   // Create kanban instance.
}
{% endhighlight %}


### getVisibleColumnNames()
{:#methods:getvisiblecolumnnames}

Used for get the names of all the visible column name collections in Kanban.

#### Returns:
{:#methods:returns:}

Array

#### Example

{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Kanban.widget.getVisibleColumnNames();      // Gets the names of all the visible column collections
} 
@ViewChild('kanban') Kanban: EJComponents<any, any>;   // Create kanban instance.
}
{% endhighlight %}


### getScrollObject()
{:#methods:getscrollobject}

Get the scroller object of Kanban.

#### Returns:
{:#methods:returns:}

ej.Scroller

#### Example

{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Kanban.widget.getScrollObject();      // Gets scroll object of Kanban control
} 
@ViewChild('kanban') Kanban: EJComponents<any, any>;   // Create kanban instance.
}
{% endhighlight %}


### getColumnByHeaderText(headerText)
{:#methods:getcolumnbyheadertext}

Get the column details based on the given header text in Kanban.

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
    <td class="name">
    headerText
    </td>
    <td class="type"><span class="param-type">string</span></td>
    <td class="description last">Pass the header text of the column to get the corresponding column object</td>
    </tr>
    </tbody>
    </table>

#### Returns:

{:#methods:returns:}

string

#### Example

{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Kanban.widget.getColumnByHeaderText("Testing");      // Gets scroll object of Kanban control
} 
@ViewChild('kanban') Kanban: EJComponents<any, any>;   // Create kanban instance.
}
{% endhighlight %}


### getHeaderTable()
{:#methods:getheadertable}

Get the table details based on the given header table in Kanban.

#### Returns:

{:#methods:returns:}

string

#### Example

{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Kanban.widget.getHeaderTable();    // Gets the table details based on the given headerTable
} 
@ViewChild('kanban') Kanban: EJComponents<any, any>;   // Create kanban instance.
}
{% endhighlight %}


### hideColumns(headerText)
{:#methods:hidecolumns}

Hide columns from the Kanban based on the header text

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
    <td class="name">
    headerText
    </td>
    <td class="type"><span class="param-type">array/string</span></td>
    <td class="description last">you can pass either array of header text of various columns or a header text of a column to hide</td>
    </tr>
    </tbody>
    </table>

#### Example

{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Kanban.widget.hideColumns("Testing");   // Hides column based on the given header text of the column
	this.Kanban.widget.hideColumns(["Testing", "Done"]); // Hide columns based on the array of header text of the columns given
} 
@ViewChild('kanban') Kanban: EJComponents<any, any>;   // Create kanban instance.
}
{% endhighlight %}


### print()
{:#methods:print}

Print the Kanban Board

#### Returns:
{:#methods:returns:}

Void

####Example

{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Kanban.widget.print();    // It prints the kanban board.
} 
@ViewChild('kanban') Kanban: EJComponents<any, any>;   // Create kanban instance.
}
{% endhighlight %}


### refreshTemplate()
{:#methods:refreshtemplate}

Refresh the template of the Kanban

#### Example

{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Kanban.widget.refreshTemplate();     // Refreshes the template of the Kanban control
} 
@ViewChild('kanban') Kanban: EJComponents<any, any>;   // Create kanban instance.
}
{% endhighlight %}


### refresh(\[templateRefresh\])
{:#methods:refresh}

Refresh the Kanban contents.The template refreshment is based on the argument passed along with this method

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
    <td class="name">
    templateRefresh
    </td>
    <td class="type"><span class="param-type">boolean</span></td>
    <td class="description last"><span class="optional">optional</span> When templateRefresh is set true, template and Kanban contents both are refreshed in Kanban else only Kanban content is refreshed</td>
    </tr>
    </tbody>
    </table>

#### Example

{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Kanban.widget.refresh();     // Refresh the Kanban contents only
	this.Kanban.widget.refresh(true);     // Refresh the template of the Kanban control
} 
@ViewChild('kanban') Kanban: EJComponents<any, any>;   // Create kanban instance.
}
{% endhighlight %}


### showColumns(headerText)
{:#methods:showcolumns}

Show columns in the Kanban based on the header text.

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
    <td class="name">
    headerText
    </td>
    <td class="type"><span class="param-type">array/string</span></td>
    <td class="description last">You can pass either array of header text of various columns or a header text of a column to show</td>
    </tr>
    </tbody>
</table>

#### Example

{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Kanban.widget.showColumns("Testing");   // Shows column based on the given header text of the column
	this.Kanban.widget.showColumns(["Testing", "Done"]); // Shows columns based on the array of header text of the columns given
} 
@ViewChild('kanban') Kanban: EJComponents<any, any>;   // Create kanban instance.
}
{% endhighlight %}


### updateCard(key,data)
{:#methods:updatecard}

Update a card in Kanban control based on key and JSON data given.

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
    <td class="name">
    key
    </td>
    <td class="type"><span class="param-type">string</span></td>
    <td class="description last">Pass the key field Name of the column</td>
    </tr>
    <tr>
    <td class="name">
    data
    </td>
    <td class="type"><span class="param-type">array</span></td>
    <td class="description last">Pass the edited JSON data of card need to be update.</td>
    </tr>
    </tbody>
    </table>

#### Example

{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Kanban.widget.updateCard(2,{ Id: 2, Status: "Open", Summary: "Task 1", Assignee: "Andrew"});   // Sends a update card request to the Kanban
} 
@ViewChild('kanban') Kanban: EJComponents<any, any>;   // Create kanban instance.
}
{% endhighlight %}


### KanbanSelection
{:#methods:kanbanselection}

### KanbanSelection.clear()
{:#methods:kanbanselection-clear}

It is used to clear all the card selection.

#### Example

{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Kanban.widget.KanbanSelection.clear();   // clears all of the card selection
} 
@ViewChild('kanban') Kanban: EJComponents<any, any>;   // Create kanban instance.
}
{% endhighlight %}


### KanbanSwimlane
{:#methods:kanbanswimlane}

### KanbanSwimlane.expandAll()
{:#methods:kanbanswimlane-expandall}

Expand all the swimlane rows in Kanban.

#### Example

{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Kanban.widget.KanbanSwimlane.expandAll();     // expand all the  rows
} 
@ViewChild('kanban') Kanban: EJComponents<any, any>;   // Create kanban instance.
}
{% endhighlight %}


### KanbanSwimlane.collapseAll()
{:#methods:kanbanswimlane-collapseall}

Collapse all the swimlane rows in Kanban.

#### Example

{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Kanban.widget.KanbanSwimlane.collapseAll();     // Collapse all the  rows
} 
@ViewChild('kanban') Kanban: EJComponents<any, any>;   // Create kanban instance.
}
{% endhighlight %}


### KanbanSwimlane.toggle($div or key)
{:#methods:kanbanswimlane-toggle}

Expand or collapse the swimlane row based on the state of target "div"

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
    <td class="name">
    $div 
    </td>
    <td class="type"><span class="param-type">object</span></td>
    <td class="description last">Pass the div object to toggleSwimlane row based on its row state</td>
    </tr>
    </tbody>
    </table>

#### Example

{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Kanban.widget.KanbanSwimlane.toggle($(".e-slexpandcollapse").eq(1));     // toggle the row based on the row state
} 
@ViewChild('kanban') Kanban: EJComponents<any, any>;   // Create kanban instance.
}
{% endhighlight %}


### KanbanFilter
{:#methods:kanbanfilter}

### KanbanFilter.clearSearch()
{:#methods:kanbanfilter-clearsearch}

Method used for send a clear search request to Kanban.

#### Example

{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Kanban.widget.KanbanFilter.clearSearch();      // Sends a clearSearch request to the Kanban
} 
@ViewChild('kanban') Kanban: EJComponents<any, any>;   // Create kanban instance.
}
{% endhighlight %}


### KanbanFilter.searchCards(searchString)
{:#methods:kanbanfilter-searchcards}

Send a search request to Kanban with specified string passed in it.

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
    <td class="type"><span class="param-type">string</span></td>
    <td class="description last">Pass the string to search in Kanban card</td>
    </tr>
    </tbody>
    </table>

#### Example

{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Kanban.widget.KanbanFilter.searchCards("Analyze");       // Sends a search request to the Kanban
} 
@ViewChild('kanban') Kanban: EJComponents<any, any>;   // Create kanban instance.
}
{% endhighlight %}


### KanbanFilter.clearFilter()
{:#methods:kanbanfilter-clearfilter}

Send a clear request to filter cards in the kanban.

#### Example

{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Kanban.widget.KanbanFilter.clearFilter();      // Sends clear request to filter the cards
} 
@ViewChild('kanban') Kanban: EJComponents<any, any>;   // Create kanban instance.
}
{% endhighlight %}


### KanbanFilter.filterCards()
{:#methods:kanbanfilter-filtercards}

Send a filtering request to cards in the kanban.

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
    <td class="name">query</td><td class="type"><span class="param-type">object</span></td>
    <td class="description last">Pass the query to the cards</td>
    </tr>
    </tbody>
    </table>

#### Example

{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Kanban.widget.KanbanFilter.filterCards(new ej.Query().where("Assignee", "equal", "Janet"));      // Sends filtering request to the cards
} 
@ViewChild('kanban') Kanban: EJComponents<any, any>;   // Create kanban instance.
}
{% endhighlight %}


### KanbanEdit
{:#methods:kanbanedit}

### KanbanEdit.addCard(\[primaryKey\],\[card\])
{:#methods:kanbanedit-addcard}

Add a new card in Kanban control when allowAdding is set as true. If parameters are not given default dialog will be open.

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
    <td class="name">primaryKey</td>
    <td class="type"><span class="param-type">string</span></td>
    <td class="description last">Pass the primary key field Name of the column</td>
    </tr>
    <tr>
    <td class="name">card</td>
    <td class="type"><span class="param-type">array</span></td>
    <td class="description last">Pass the edited JSON data of card need to be add.</td>
    </tr>
    </tbody>
    </table>

#### Example

{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Kanban.widget.KanbanEdit.addCard();      // Sends an add new card request to the Kanban
} 
@ViewChild('kanban') Kanban: EJComponents<any, any>;   // Create kanban instance.
}
{% endhighlight %}


### KanbanEdit.cancelEdit()
{:#methods:kanbanedit-canceledit}

Send a cancel request of add/edit card in Kanban when allowEditing/allowAdding is set as true.

#### Example

{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Kanban.widget.KanbanEdit.cancelEdit();      // Sends a cancel request to the Kanban
} 
@ViewChild('kanban') Kanban: EJComponents<any, any>;   // Create kanban instance.
}
{% endhighlight %}


### KanbanEdit.deleteCard(Key)
{:#methods:kanbanedit-deletecard}

Delete a card in Kanban control when allowAdding/allowEditing is set as true.

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
    <td class="name">Key</td>
    <td class="type"><span class="param-type">string/number</span></td>
    <td class="description last">Pass the key of card to be delete</td>
    </tr>
    </tbody>
    </table>

#### Example

{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Kanban.widget.KanbanEdit.deleteCard(2);     // Sends a delete card request to the Kanban
} 
@ViewChild('kanban') Kanban: EJComponents<any, any>;   // Create kanban instance.
}
{% endhighlight %}


### KanbanEdit.endEdit()
{:#methods:kanbanedit-endedit}

Send a save request in Kanban when any card is in edit/new add card state and allowEditing/allowAdding is set as true.

#### Example

{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Kanban.widget.KanbanEdit.endEdit();     // Sends a save request to the Kanban
} 
@ViewChild('kanban') Kanban: EJComponents<any, any>;   // Create kanban instance.
}
{% endhighlight %}


### KanbanEdit.startEdit($div or key)
{:#methods:kanbanedit-startedit}

Send an edit card request in Kanban when allowEditing is set as true. Parameter will be HTML element or primary key

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
    <td class="name">
    $div
    </td>
    <td class="type"><span class="param-type">object</span></td>
    <td class="description last">Pass the div selected row element to be edited in Kanban</td>
    </tr>
    <td class="name">
    key
    </td>
    <td class="type"><span class="param-type">string/number</span></td>
    <td class="description last">Pass the key element to be edited in Kanban</td>
    </tr>
    </tbody>
    </table>

#### Example

{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Kanban.widget.KanbanEdit.startEdit($(".e-kanbancontent .e-kanbancard").first());      // Sends an edit card request to the Kanban
	this.Kanban.widget.KanbanEdit.startEdit(2);
} 
@ViewChild('kanban') Kanban: EJComponents<any, any>;   // Create kanban instance.
}
{% endhighlight %}


### KanbanEdit.setValidationToField(name, rules)
{:#methods:kanbanedit-setvalidationtofield}

Method used for set validation to a field during editing.

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
     <td class="name">name</td>
    <td class="type"><span class="param-type">string</span></td>
    <td class="description last">Specify the name of the column to set validation rules</td>
    </tr>
    <tr>
    <td class="name">rules</td>
    <td class="type"><span class="param-type">object</span></td>
    <td class="description last">Specify the validation rules for the field</td>
    </tr>
    </tbody>
    </table>

#### Example

{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Kanban.widget.KanbanEdit.setValidationToField("Summary", { required: true });       // It is used to set validation to a field during editing
} 
@ViewChild('kanban') Kanban: EJComponents<any, any>;   // Create kanban instance.
}
{% endhighlight %}


## Events

### actionBegin
{:#events:actionbegin}

Triggered for every Kanban action before its starts.
    
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
        <td class="name">argument</td>
        <td class="type"><span class="param-type">Object</span></td>
        <td class="description last">Event parameters when Kanban is initialized:
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
        <td class="name">model</td>
        <td class="type"><span class="param-type">object</span></td>
        <td class="description last">Returns the Kanban model.</td>
        </tr>
        <tr>
        <td class="name">type</td>
        <td class="type"><span class="param-type">string</span></td>
        <td class="description last">Returns the name of the event.</td>
        </tr>
        </tbody>
        </table>
        </td>
        </tr>
        <tr>
        <td class="name">argument</td>
        <td class="type"><span class="param-type">Object</span></td>
        <td class="description last">Event parameters when Kanban card editing action starts:
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
        <td class="description last">Returns the cancel option value.</td>
        </tr>
        <tr>
        <td class="name">model</td>
        <td class="type"><span class="param-type">object</span></td>
        <td class="description last">Returns the Kanban model.</td>
        </tr>
        <tr>
        <td class="name">originalEventType</td>
        <td class="type"><span class="param-type">string</span></td>
        <td class="description last">Returns the current action event type.</td>
        </tr>
        <tr>
        <td class="name">primaryKeyValue</td>
        <td class="type"><span class="param-type">string</span></td>
        <td class="description last">Returns primary key value.</td>
        </tr>
        <tr>
        <td class="name">requestType</td>
        <td class="type"><span class="param-type">string</span></td>
        <td class="description last">Returns request type.</td>
        </tr>
        <tr>
        <td class="name">rowIndex</td>
        <td class="type"><span class="param-type">number</span></td>
        <td class="description last">Returns the edited row index.</td>
        </tr>
        <tr>
        <td class="name">type</td>
        <td class="type"><span class="param-type">string</span></td>
        <td class="description last">Returns the name of the event.</td>
        </tr>
        </tbody>
        </table>
        </td>
        </tr>
        <tr>
        <td class="name">argument</td>
        <td class="type"><span class="param-type">Object</span></td>
        <td class="description last">Event parameters when Kanban card save action starts:
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
        <td class="description last">Returns the cancel option value.</td>
        </tr>
        <tr>
        <td class="name">data</td>
        <td class="type"><span class="param-type">object</span></td>
        <td class="description last">Returns the card object (JSON).</td>
        </tr>
        <tr>
        <td class="name">model</td>
        <td class="type"><span class="param-type">object</span></td>
        <td class="description last">Returns the Kanban model.</td>
        </tr>
        <tr>
        <td class="name">primaryKeyValue</td>
        <td class="type"><span class="param-type">string</span></td>
        <td class="description last">Returns primary key value.</td>
        </tr>
        <tr>
        <td class="name">requestType</td>
        <td class="type"><span class="param-type">string</span></td>
        <td class="description last">Returns request type.</td>
        </tr>
        <tr>
        <td class="name">type</td>
        <td class="type"><span class="param-type">string</span></td>
        <td class="description last">Returns the name of the event.</td>
        </tr>
        </tbody>
        </table>
        </td>
        </tr>
        <tr>
        <td class="name">argument</td>
        <td class="type"><span class="param-type">Object</span></td>
        <td class="description last">Event parameters when Kanban card cancel action starts:
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
        <td class="description last">Returns the cancel option value.</td>
        </tr>
        <tr>
        <td class="name">model</td>
        <td class="type"><span class="param-type">object</span></td>
        <td class="description last">Returns the Kanban model.</td>
        </tr>
        <tr>
        <td class="name">requestType</td>
        <td class="type"><span class="param-type">string</span></td>
        <td class="description last">Returns request type.</td>
        </tr>
        <tr>
        <td class="name">type</td>
        <td class="type"><span class="param-type">string</span></td>
        <td class="description last">Returns the name of the event.</td>
        </tr>
        </tbody>
        </table>
        </td>
        </tr>
        <tr>
        <td class="name">argument</td>
        <td class="type"><span class="param-type">Object</span></td>
        <td class="description last">Event parameters when Kanban card delete action starts:
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
        <td class="description last">Returns the cancel option value.</td>
        </tr>
        <tr>
        <td class="name">data</td>
        <td class="type"><span class="param-type">object</span></td>
        <td class="description last">Returns the card object (JSON).</td>
        </tr>
        <tr>
        <td class="name">model</td>
        <td class="type"><span class="param-type">object</span></td>
        <td class="description last">Returns the Kanban model.</td>
        </tr>
        <tr>
        <td class="name">requestType</td>
        <td class="type"><span class="param-type">string</span></td>
        <td class="description last">Returns request type.</td>
        </tr>
        <tr>
        <td class="name">type</td>
        <td class="type"><span class="param-type">string</span></td>
        <td class="description last">Returns the name of the event.</td>
        </tr>
        </tbody>
        </table>
        </td>
        </tr>
        <tr>
        <td class="name">argument</td>
        <td class="type"><span class="param-type">Object</span></td>
        <td class="description last">Event parameters when add new card action starts:
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
        <td class="description last">Returns the cancel option value.</td>
        </tr>
        <tr>
        <td class="name">data</td>
        <td class="type"><span class="param-type">object</span></td>
        <td class="description last">Returns the card object (JSON).</td>
        </tr>
        <tr>
        <td class="name">model</td>
        <td class="type"><span class="param-type">object</span></td>
        <td class="description last">Returns the Kanban model.</td>
        </tr>
        <tr>
        <td class="name">requestType</td>
        <td class="type"><span class="param-type">string</span></td>
        <td class="description last">Returns request type as `add`.</td>
        </tr>
        <tr>
        <td class="name">type</td>
        <td class="type"><span class="param-type">string</span></td>
        <td class="description last">Returns the name of the event.</td>
        </tr>
        </tbody>
        </table>
        </td>
        </tr>
        <tr>
        <td class="name">argument</td>
        <td class="type"><span class="param-type">Object</span></td>
        <td class="description last">Event parameters when Kanban filtering action starts:
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
        <td class="description last">Returns the cancel option value.</td>
        </tr>
        <tr>
        <td class="name">currentFiltering object</td>
        <td class="type"><span class="param-type">object</span></td>
        <td class="description last">Returns current filtering object field name.</td>
        </tr>
        <tr>
        <td class="name">filterCollection</td>
        <td class="type"><span class="param-type">object</span></td>
        <td class="description last">Returns filter details.</td>
        </tr>
        <tr>
        <td class="name">model</td>
        <td class="type"><span class="param-type">object</span></td>
        <td class="description last">Returns the Kanban model.</td>
        </tr>
        <tr>
        <td class="name">requestType</td>
        <td class="type"><span class="param-type">string</span></td>
        <td class="description last">Returns request type.</td>
        </tr>
        <tr>
        <td class="name">type</td>
        <td class="type"><span class="param-type">string</span></td>
        <td class="description last">Returns the name of the event.</td>
        </tr>
        </tbody>
        </table>
        </td>
        </tr>
        </tbody>
        </table>

#### Example

{% highlight html %}

    <ej-kanban id="kanban" [dataSource]="kanbanData" (actionBegin)="onActionBegin($event)"> 

{% endhighlight %}

{% highlight ts %}

    onActionBegin(e: any){ 
         // Your code here
    }

{% endhighlight %}


### actionComplete
{:#events:actioncomplete}

Triggered for every Kanban action success event.

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
    <td class="name">argument</td>
    <td class="type"><span class="param-type">Object</span></td>
    <td class="description last">Arguments in actionComplete when Kanban is initialized.
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
    <td class="description last">Returns the cancel option value.</td>
    </tr>
    <tr>
    <td class="name">model</td>
    <td class="type"><span class="param-type">object</span></td>
    <td class="description last">Returns the Kanban model.</td>
    </tr>
    <tr>
    <td class="name">requestType</td>
    <td class="type"><span class="param-type">string</span></td>
    <td class="description last">Returns request type.</td>
    </tr>
    <tr>
    <td class="name">type</td>
    <td class="type"><span class="param-type">string</span></td>
    <td class="description last">Returns the name of the event.</td>
    </tr>
    </tbody>
    </table>
    </td>
    </tr>
    <tr>
    <td class="name">argument</td>
    <td class="type"><span class="param-type">object</span></td>
    <td class="description last">Arguments in actionComplete after Kanban card editing action is completed.
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
    <td class="description last">Returns the cancel option value.</td>
    </tr>
    <tr>
    <td class="name">model</td>
    <td class="type"><span class="param-type">object</span></td>
    <td class="description last">Returns the Kanban model.</td>
    </tr>
    <tr>
    <td class="name">originalEventType</td>
    <td class="type"><span class="param-type">string</span></td>
    <td class="description last">Returns current action event type.</td>
    </tr>
    <tr>
    <td class="name">primaryKey</td>
    <td class="type"><span class="param-type">string</span></td>
    <td class="description last">Returns primary key.</td>
    </tr>
    <tr>
    <td class="name">primaryKeyValue</td>
    <td class="type"><span class="param-type">string</span></td>
    <td class="description last">Returns primary key value.</td>
    </tr>
    <tr>
    <td class="name">requestType</td>
    <td class="type"><span class="param-type">string</span></td>
    <td class="description last">Returns request type.</td>
    </tr>
    <tr>
    <td class="name">target</td>
    <td class="type"><span class="param-type">object</span></td>
    <td class="description last">Returns Kanban element.</td>
    </tr>
    <tr>
    <td class="name">type</td>
    <td class="type"><span class="param-type">string</span></td>
    <td class="description last">Returns the name of the event.</td>
    </tr>
    </tbody>
    </table>
    </td>
    </tr>
    <tr>
    <td class="name">argument</td>
    <td class="type"><span class="param-type">object</span></td>
    <td class="description last">Arguments in actionComplete after Kanban card save action is completed.
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
    <td class="type"><span class="param-type">object</span></td>
    <td class="description last">Returns the cancel option value.</td>
    </tr>
    <tr>
    <td class="name">data</td>
    <td class="type"><span class="param-type">object</span></td>
    <td class="description last">Returns the card object (JSON).</td>
    </tr>
    <tr>
    <td class="name">selectedRow</td>
    <td class="type"><span class="param-type">number</span></td>
    <td class="description last">Returns the selectedRow index.</td>
    </tr>
    <tr>
    <td class="name">model</td>
    <td class="type"><span class="param-type">object</span></td>
    <td class="description last">Returns the Kanban model.</td>
    </tr>
    <tr>
    <td class="name">originalEventType</td>
    <td class="type"><span class="param-type">string</span></td>
    <td class="description last">Returns current action event type.</td>
    </tr>
    <tr>
    <td class="name">requestType</td>
    <td class="type"><span class="param-type">string</span></td>
    <td class="description last">Returns request type.</td>
    </tr>
    <tr>
    <td class="name">target</td>
    <td class="type"><span class="param-type">object</span></td>
    <td class="description last">Returns Kanban element.</td>
    </tr>
    <tr>
    <td class="name">type</td>
    <td class="type"><span class="param-type">string</span></td>
    <td class="description last">Returns the name of the event.</td>
    </tr>
    </tbody>
    </table>
    </td>
    </tr>
    <tr>
    <td class="name">argument</td>
    <td class="type"><span class="param-type">object</span></td>
    <td class="description last">Arguments in actionComplete after Kanban card cancel action is completed.
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
    <td class="description last">Returns the cancel option value.</td>
    </tr>
    <tr>
    <td class="name">model</td>
    <td class="type"><span class="param-type">object</span></td>
    <td class="description last">Returns the Kanban model.</td>
    </tr>
    <tr>
    <td class="name">originalEventType</td>
    <td class="type"><span class="param-type">string</span></td>
    <td class="description last">Returns current action event type.</td>
    </tr>
    <tr>
    <td class="name">requestType</td>
    <td class="type"><span class="param-type">string</span></td>
    <td class="description last">Returns request type.</td>
    </tr>
    <tr>
    <td class="name">target</td>
    <td class="type"><span class="param-type">object</span></td>
    <td class="description last">Returns Kanban element.</td>
    </tr>
    <tr>
    <td class="name">type</td>
    <td class="type"><span class="param-type">string</span></td>
    <td class="description last">Returns the name of the event.</td>
    </tr>
    </tbody>
    </table>
    </td>
    </tr>
    <tr>
    <td class="name">argument</td>
    <td class="type"><span class="param-type">object</span></td>
    <td class="description last">Arguments in actionComplete after Kanban card delete action is completed.
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
    <td class="description last">Returns the cancel option value.</td>
    </tr>
    <tr>
    <td class="name">data</td>
    <td class="type"><span class="param-type">object</span></td>
    <td class="description last">Returns the card object (JSON).</td>
    </tr>
    <tr>
    <td class="name">model</td>
    <td class="type"><span class="param-type">object</span></td>
    <td class="description last">Returns the Kanban model.</td>
    </tr>
    <tr>
    <td class="name">originalEventType</td>
    <td class="type"><span class="param-type">string</span></td>
    <td class="description last">Returns current action event type.</td>
    </tr>
    <tr>
    <td class="name">requestType</td>
    <td class="type"><span class="param-type">string</span></td>
    <td class="description last">Returns request type.</td>
    </tr>
    <tr>
    <td class="name">target</td>
    <td class="type"><span class="param-type">object</span></td>
    <td class="description last">Returns Kanban element.</td>
    </tr>
    <tr>
    <td class="name">type</td>
    <td class="type"><span class="param-type">string</span></td>
    <td class="description last">Returns the name of the event.</td>
    </tr>
    </tbody>
    </table>
    </td>
    </tr>
    <tr>
    <td class="name">argument</td>
    <td class="type"><span class="param-type">object</span></td>
    <td class="description last">Arguments in actionComplete after add new card action is completed.
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
    <td class="description last">Returns the cancel option value.</td>
    </tr>
    <tr>
    <td class="name">data</td>
    <td class="type"><span class="param-type">object</span></td>
    <td class="description last">Returns empty card object (JSON).</td>
    </tr>
    <tr>
    <td class="name">model</td>
    <td class="type"><span class="param-type">object</span></td>
    <td class="description last">Returns the Kanban model.</td>
    </tr>
    <tr>
    <td class="name">originalEventType</td>
    <td class="type"><span class="param-type">string</span></td>
    <td class="description last">Returns current action event type.</td>
    </tr>
    <tr>
    <td class="name">requestType</td>
    <td class="type"><span class="param-type">string</span></td>
    <td class="description last">Returns request type.</td>
    </tr>
    <tr>
    <td class="name">target</td>
    <td class="type"><span class="param-type">object</span></td>
    <td class="description last">Returns Kanban element.</td>
    </tr>
    <tr>
    <td class="name">type</td>
    <td class="type"><span class="param-type">string</span></td>
    <td class="description last">Returns the name of the event.</td>
    </tr>
    </tbody>
    </table>
    </td>
    </tr>
    <tr>
    <td class="name">argument</td>
    <td class="type"><span class="param-type">object</span></td>
    <td class="description last">Arguments in actionComplete after Kanban filtering action is completed.
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
    <td class="description last">Returns the cancel option value.</td>
    </tr>
    <tr>
    <td class="name">currentFilteringColumn</td>
    <td class="type"><span class="param-type">string</span></td>
    <td class="description last">Returns current filtering column field name.</td>
    </tr>
    <tr>
    <td class="name">filterCollection</td>
    <td class="type"><span class="param-type">object</span></td>
    <td class="description last">Returns filter details.</td>
    </tr>
    <tr>
    <td class="name">model</td>
    <td class="type"><span class="param-type">object</span></td>
    <td class="description last">Returns the Kanban model.</td>
    </tr>
    <tr>
    <td class="name">originalEventType</td>
    <td class="type"><span class="param-type">string</span></td>
    <td class="description last">Returns current action event type.</td>
    </tr>
    <tr>
    <td class="name">requestType</td>
    <td class="type"><span class="param-type">string</span></td>
    <td class="description last">Returns request type.</td>
    </tr>
    <tr>
    <td class="name">target</td>
    <td class="type"><span class="param-type">object</span></td>
    <td class="description last">Returns Kanban element.</td>
    </tr>
    <tr>
    <td class="name">type</td>
    <td class="type"><span class="param-type">string</span></td>
    <td class="description last">Returns the name of the event.</td>
    </tr>
    </tbody>
    </table>
    </td>
    </tr>
    </tbody>
</table>

#### Example

{% highlight html %}

    <ej-kanban id="kanban" [dataSource]="kanbanData" (actionComplete)="onActionComplete($event)"> 

{% endhighlight %}

{% highlight ts %}

    onActionComplete(e: any){ 
         // Your code here
    }

{% endhighlight %}


### actionFailure
{:#events:actionfailure}

Triggered for every Kanban action server failure event.

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
<td class="name">argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Arguments in actionFailure when Kanban is initialized.
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the Kanban model.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns request type.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">error</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the error return by server.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Arguments in actionFailure after Kanban card editing action is completed.
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the Kanban model.</td>
</tr>
<tr>
<td class="name">originalEventType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns current action event type.</td>
</tr>
<tr>
<td class="name">primaryKeyValue</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns primary key value.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns request type.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns Kanban element.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">error</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the error return by server.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Arguments in actionFailure after Kanban card save action is completed.
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
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the card object (JSON).</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the Kanban model.</td>
</tr>
<tr>
<td class="name">originalEventType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns current action event type.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns request type.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns Kanban element.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">error</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the error return by server.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Arguments in actionFailure after Kanban card delete action is completed.
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the card object (JSON).</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the Kanban model.</td>
</tr>
<tr>
<td class="name">originalEventType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns current action event type.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns request type.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns Kanban element.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">error</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the error return by server.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Arguments in actionFailure after add new card action is completed.
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns empty card object (JSON).</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the Kanban model.</td>
</tr>
<tr>
<td class="name">originalEventType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns current action event type.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns request type.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns Kanban element.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">error</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the error return by server.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Arguments in actionFailure after Kanban filtering action is completed.
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">currentFilteringColumn</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns current filtering column field name.</td>
</tr>
<tr>
<td class="name">filterCollection</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns filter details.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the Kanban model.</td>
</tr>
<tr>
<td class="name">originalEventType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns current action event type.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns request type.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns Kanban element.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">error</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the error return by server.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

    <ej-kanban id="kanban" [dataSource]="kanbanData" (actionFailure)="onActionFailure($event)"> 

{% endhighlight %}

{% highlight ts %}

    onActionFailure(e: any){ 
         // Your code here
    }

{% endhighlight %}


### beginEdit
{:#events:beginedit}

Triggered before the task is going to be edited.

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
<td class="name">argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Arguments when begin edit event is triggered.
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the Kanban model.</td>
</tr>
<tr>
<td class="name">primaryKeyValue</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns primary key value.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns begin edit data.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

    <ej-kanban id="kanban" [dataSource]="kanbanData" (beginEdit)="onBeginEdit($event)"> 

{% endhighlight %}

{% highlight ts %}

    onBeginEdit(e: any){ 
         // Your code here
    }

{% endhighlight %}


### beforeCardSelect
{:#events:beforecardselect}

Triggered before the card is selected.

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
<td class="name">argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Arguments when beforeCardSelect event is triggered.
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">cellIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the select cell index value.</td>
</tr>
<tr>
<td class="name">cardIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the select card index value.</td>
</tr>
<tr>
<td class="name">currentCell</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the select cell element</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">previousCard</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the previously select the card element</td>
</tr>
<tr>
<td class="name">previous Row cell index</td>
<td class="type"><span class="param-type">array</span></td>
<td class="description last">Returns the previously select card indexes</td>
</tr>
<tr>
<td class="name">Target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the Target item.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the Kanban model.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns select card data.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

    <ej-kanban id="kanban" [dataSource]="kanbanData" (beforeCardSelect)="onBeforeCardSelect($event)"> 

{% endhighlight %}

{% highlight ts %}

    onBeforeCardSelect(e: any){ 
         // Your code here
    }

{% endhighlight %}


### cardClick
{:#events:cardclick}

Trigger after the card is clicked.

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
<td class="name">argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Arguments when cardClick event is triggered.
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns current record object (JSON).</td>
</tr>
<tr>
<td class="name">currentCard</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the current card to the Kanban.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns Kanban element.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the Kanban model.</td>
</tr>
<tr>
<td class="name">columnName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the Header text of the column corresponding to the selected card.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

    <ej-kanban id="kanban" [dataSource]="kanbanData" (cardClick)="onCardClick($event)"> 

{% endhighlight %}

{% highlight ts %}

    onCardClick(e: any){ 
         // Your code here
    }

{% endhighlight %}


### cardDrag
{:#events:carddrag}

Triggered when the card is being dragged.

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
<td class="name">argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Arguments when columnDrag event is triggered.
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns drag data.</td>
</tr>
<tr>
<td class="name">drag target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns drag start element.</td>
</tr>
<tr>
<td class="name">draggedElement</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns dragged element.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the Kanban model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

    <ej-kanban id="kanban" [dataSource]="kanbanData" (cardDrag)="onCardDrag($event)"> 

{% endhighlight %}

{% highlight ts %}

    onCardDrag(e: any){ 
         // Your code here
    }

{% endhighlight %}


### cardDragStart
{:#events:carddragstart}

Triggered when card dragging start.

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
<td class="name">argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Arguments when cardDragStart event is triggered.
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns card drag start data.</td>
</tr>
<tr>
<td class="name">draggedElement</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns dragged element.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the Kanban model.</td>
</tr>
<tr>
<td class="name">drag target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns drag start element.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

    <ej-kanban id="kanban" [dataSource]="kanbanData" (cardDragStart)="onCardDragStart($event)"> 

{% endhighlight %}

{% highlight ts %}

    onCardDragStart(e: any){ 
         // Your code here
    }

{% endhighlight %}


### cardDragStop
{:#events:carddragstop}

Triggered when card dragging stops.

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
<td class="name">argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Arguments when cardDragStart event is triggered.
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">draggedElement</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns dragged element.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the Kanban model.</td>
</tr>
<tr>
<td class="name">drop target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns drag stop element.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns drag stop data.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

    <ej-kanban id="kanban" [dataSource]="kanbanData" (cardDragStop)="onCardDragStop($event)"> 

{% endhighlight %}

{% highlight ts %}

    onCardDragStop(e: any){ 
         // Your code here
    }

{% endhighlight %}


### cardDrop
{:#events:carddrop}

Triggered when the card is Dropped.

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
<td class="name">argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Arguments when cardDrop event is triggered.
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">draggedElement</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns dragged element.</td>
</tr>
<tr>
<td class="name">draggedParent</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns previous parent of dragged element</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns dragged data.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the Kanban model.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns drop element.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

    <ej-kanban id="kanban" [dataSource]="kanbanData" (cardDrop)="onCardDrop($event)"> 

{% endhighlight %}

{% highlight ts %}

    onCardDrop(e: any){ 
         // Your code here
    }

{% endhighlight %}


### cardSelect
{:#events:cardselect}

Triggered after the card is selected.

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
<td class="name">argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Arguments when cardSelect event is triggered.
<table class="params">
<thead
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">cellIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the select cell index value.</td>
</tr>
<tr>
<td class="name">cardIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the select card index value.</td>
</tr>
<tr>
<td class="name">currentCell</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the select cell element</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">previousCard</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the previously select the card element</td>
</tr>
<tr>
<td class="name">previous Row cell index</td>
<td class="type"><span class="param-type">array</span></td>
<td class="description last">Returns the previously select card indexes</td>
</tr>
<tr>
<td class="name">currentTarget</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the current item.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the Kanban model.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns select card data.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

    <ej-kanban id="kanban" [dataSource]="kanbanData" (cardSelect)="onCardSelect($event)"> 

{% endhighlight %}

{% highlight ts %}

    onCardSelect(e: any){ 
         // Your code here
    }

{% endhighlight %}


### cardDoubleClick
{:#events:carddoubleclick}

Triggered when card is double clicked.

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
                <td class="name">argument</td>
                <td class="type"><span class="param-type">Object</span></td>
                <td class="description last">
                    Arguments when cardDoubleClick event is triggered.
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
                                <td class="description last">Returns the cancel option value.</td>
                            </tr>
                            <tr>
                                <td class="name">data</td>
                                <td class="type"><span class="param-type">object</span></td>
                                <td class="description last">Returns current card object (JSON).</td>
                            </tr>
                            <tr>
                                <td class="name">model</td>
                                <td class="type"><span class="param-type">object</span></td>
                                <td class="description last">Returns the Kanban model.</td>
                            </tr>
                            <tr>
                                <td class="name">type</td>
                                <td class="type"><span class="param-type">string</span></td>
                                <td class="description last">Returns the name of the event.</td>
                            </tr>
                        </tbody>
                    </table>
                </td>
            </tr>
        </tbody>
    </table>

#### Example

{% highlight html %}

    <ej-kanban id="kanban" [dataSource]="kanbanData" (cardDoubleClick)="onCardDoubleClick($event)"> 

{% endhighlight %}

{% highlight ts %}

    onCardDoubleClick(e: any){ 
         // Your code here
    }

{% endhighlight %}


### cardSelecting
{:#events:cardselecting}

Triggered before the card is selected.

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
<td class="name">argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Arguments when cardSelecting event is triggered.
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
<td class="name">cellIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the selecting cell index value.</td>
</tr>
<tr>
<td class="name">cardIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the selecting card index value.</td>
</tr>
<tr>
<td class="name">currentCell</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the selecting cell element</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">previousCard</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the previously selecting the card element</td>
</tr>
<tr>
<td class="name">previous Row cell index</td>
<td class="type"><span class="param-type">array</span></td>
<td class="description last">Returns the previously row cell is selecting card indexes</td>
</tr>
<tr>
<td class="name">currentTarget</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the current item.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the Kanban model.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns added data.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

    <ej-kanban id="kanban" [dataSource]="kanbanData" (cardSelecting)="onCardSelecting($event)"> 

{% endhighlight %}

{% highlight ts %}

    onCardSelecting(e: any){ 
         // Your code here
    }

{% endhighlight %}


### create
{:#events:create}

Triggered when the Kanban is rendered completely

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Kanban.Model"/><span class="param-type">Object</span></td>
<td class="description last">Event parameters from kanban
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the kanban model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

    <ej-kanban id="kanban" [dataSource]="kanbanData" (create)="onCreate($event)"> 

{% endhighlight %}

{% highlight ts %}

    onCreate(e: any){ 
         // Your code here
    }

{% endhighlight %}


### cellClick
{:#events:cellclick}

Triggers after the cell is clicked.

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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type">object</td>
<td class="description">Returns the kanban model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type">string</td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">cellIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the select cell index value.</td>
</tr>
<tr>
<td class="name">rowIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the edited row index.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

    <ej-kanban id="kanban" [dataSource]="kanbanData" (cellClick)="onCellClick($event)"> 

{% endhighlight %}

{% highlight ts %}

    onCellClick(e: any){ 
         // Your code here
    }

{% endhighlight %}


### contextOpen
{:#events:contextopen}

Triggered before the context menu is opened.

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
<td class="name">argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">
Arguments when contextOpen event is triggered.
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the Kanban model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">currentTarget</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the current item.</td>
</tr>
<tr>
<td class="name">status</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Returns the status of context menu item which denotes its enabled state.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the target item.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

    <ej-kanban id="kanban" [dataSource]="kanbanData"  (contextOpen)="onContextOpen($event)"> 

{% endhighlight %}

{% highlight ts %}

    onContextOpen(e: any){ 
         // Your code here
    }

{% endhighlight %}


### contextClick
{:#events:contextclick}

Triggered when context menu item is clicked in Kanban

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
<td class="name">argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">
Arguments when contextClick event is triggered
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the Kanban model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">currentTarget</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the current item.</td>
</tr>
<tr>
<td class="name">status</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Returns the status of context menu item which denotes its enabled state.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the target item.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

    <ej-kanban id="kanban" [dataSource]="kanbanData"  (contextClick)="onContextClick($event)"> 

{% endhighlight %}

{% highlight ts %}

    onContextClick(e: any){ 
         // Your code here
    }

{% endhighlight %}


### dataBound
{:#events:databound}

Triggered the Kanban is bound with data during initial rendering.

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
<td class="name">argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Arguments when dataBound event is triggered.
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the Kanban model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

    <ej-kanban id="kanban" [dataSource]="kanbanData"  (dataBound)="onDataBound($event)"> 

{% endhighlight %}

{% highlight ts %}

    onDataBound(e: any){ 
         // Your code here
    }

{% endhighlight %}


### destroy
{:#events:destroy}

Triggered when Kanban going to destroy.  

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Kanban.Model"/><span class="param-type">Object</span></td>
<td class="description last">Arguments when destroy event is triggered.
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
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the kanban model.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns deleted data.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

    <ej-kanban id="kanban" [dataSource]="kanbanData"  (destroy)="onDestroy($event)"> 

{% endhighlight %}

{% highlight ts %}

    onDestroy(e: any){ 
         // Your code here
    }

{% endhighlight %}


### endDelete
{:#events:enddelete}

Triggered after the card is deleted.

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
<td class="name">argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Arguments when endDelete event is triggered.
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
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the Kanban model.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns request type.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns deleted  data.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">action</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Current action name</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

    <ej-kanban id="kanban" [dataSource]="kanbanData"  (endDelete)="onEndDelete($event)"> 

{% endhighlight %}

{% highlight ts %}

    onEndDelete(e: any){ 
         // Your code here
    }

{% endhighlight %}


### endEdit
{:#events:endedit}

Triggered after the card is edited.

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
<td class="name">argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Arguments when endEdit event is triggered.
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
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the Kanban model.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns request type.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns modified data.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">action</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Current Action name</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

    <ej-kanban id="kanban" [dataSource]="kanbanData"  (endEdit)="onEndEdit($event)"> 

{% endhighlight %}

{% highlight ts %}

    onEndEdit(e: any){ 
         // Your code here
    }

{% endhighlight %}


### headerClick
{:#events:headerclick}

Triggers after the header is clicked.

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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type">object</td>
<td class="description">Returns the kanban model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type">string</td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">cellIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the select cell index value.</td>
</tr>
<tr>
<td class="name">columnData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the column object.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

    <ej-kanban id="kanban" [dataSource]="kanbanData"  (headerClick)="onHeaderClick($event)"> 

{% endhighlight %}

{% highlight ts %}

    onHeaderClick(e: any){ 
         // Your code here
    }

{% endhighlight %}


### load
{:#events:load}

Triggered initial load.

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Kanban.Model"/><span class="param-type">Object</span></td>
<td class="description last">Arguments when load event is triggered.
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
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the kanban model.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

    <ej-kanban id="kanban" [dataSource]="kanbanData" (load)="onLoad($event)"> 

{% endhighlight %}

{% highlight ts %}

    onLoad(e: any){ 
         // Your code here
    }

{% endhighlight %}


### swimlaneClick
{:#events:swimlaneclick}

Triggers before swim lane expand or collapse icon is clicked.

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Kanban.Model"/><span class="param-type">Object</span></td>
<td class="description last">Arguments when swim lane click event is triggered.
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
<td class="name">action</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Current Action name while swim lane clicked. Actions are "expand" or "collapse"</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the kanban model.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the swim lane group data's.</td>
</tr>
<tr>
<td class="name">rowIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns current swim lane row index.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns current target element.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

    <ej-kanban id="kanban" [dataSource]="kanbanData" (swimlaneClick)="onSwimlaneClick($event)"> 

{% endhighlight %}

{% highlight ts %}

    onSwimlaneClick(e: any){ 
         // Your code here
    }

{% endhighlight %}


### queryCellInfo
{:#events:querycellinfo}

Triggered every time a single card rendered request is made to access particular card information.

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
        <td class="name">argument</td>
        <td class="type"><span class="param-type">Object</span></td>
        <td class="description last">
        Event parameters from Kanban
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
        <td class="name">card</td>
        <td class="type"><span class="param-type">object</span></td>
        <td class="description last">Returns Kanban card.</td>
        </tr>
        <tr>
        <td class="name">cell</td>
        <td class="type"><span class="param-type">object</span></td>
        <td class="description last">Returns Kanban card.</td>
        </tr>
        <tr>
        <td class="name">cancel</td>
        <td class="type"><span class="param-type">boolean</span></td>
        <td class="description last">Returns the cancel option value.</td>
        </tr>
        <tr>
        <td class="name">data</td>
        <td class="type"><span class="param-type">object</span></td>
        <td class="description last">Returns current row record object (JSON).</td>
        </tr>
        <tr>
        <td class="name">column</td>
        <td class="type"><span class="param-type">object</span></td>
        <td class="description last">Returns the column object.</td>
        </tr>
        <tr>
        <td class="name">model</td>
        <td class="type"><span class="param-type">object</span></td>
        <td class="description last">Returns the Kanban model.</td>
        </tr>
        <tr>
        <td class="name">type</td>
        <td class="type"><span class="param-type">string</span></td>
        <td class="description last">Returns the name of the event.</td>
        </tr>
        </tbody>
        </table>
        </td>
        </tr>
        </tbody>
</table>

#### Example

{% highlight html %}

    <ej-kanban id="kanban" [dataSource]="kanbanData" (queryCellInfo)="onQueryCellInfo($event)"> 

{% endhighlight %}

{% highlight ts %}

    onQueryCellInfo(e: any){ 
         // Your code here
    }

{% endhighlight %}


### toolbarClick
{:#events:toolbarclick}

Triggered when toolbar item is clicked in Kanban.
    
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
                <td class="name">argument</td>
                <td class="type"><span class="param-type">Object</span></td>
                <td class="description last">
                    Arguments when toolBarClick event is triggered.
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
                                <td class="description last">Returns the cancel option value.</td>
                            </tr>
                            <tr>
                                <td class="name">currentTarget</td>
                                <td class="type"><span class="param-type">object</span></td>
                                <td class="description last">Returns the current item.</td>
                            </tr>
                            <tr>
                                <td class="name">itemId</td>
                                <td class="type"><span class="param-type">string</span></td>
                                <td class="description last">Returns the item id of that current element.</td>
                            </tr>
                            <tr>
                                <td class="name">itemIndex</td>
                                <td class="type"><span class="param-type">number</span></td>
                                <td class="description last">Returns the item index of that current element.</td>
                            </tr>
                            <tr>
                                <td class="name">itemName</td>
                                <td class="type"><span class="param-type">string</span></td>
                                <td class="description last">Returns the item name of that current element.</td>
                            </tr>
                            <tr>
                                <td class="name">itemText</td>
                                <td class="type"><span class="param-type">string</span></td>
                                <td class="description last">Returns the item text of that current element.</td>
                            </tr>
                            <tr>
                                <td class="name">model</td>
                                <td class="type"><span class="param-type">object</span></td>
                                <td class="description last">Returns the Kanban model.</td>
                            </tr>
                            <tr>
                                <td class="name">type</td>
                                <td class="type"><span class="param-type">string</span></td>
                                <td class="description last">Returns the name of the event.</td>
                            </tr>
                            <tr>
                                <td class="name">toolbarData</td>
                                <td class="type"><span class="param-type">object</span></td>
                                <td class="description last">Returns the toolbar object of the Kanban.</td>
                            </tr>
                        <tbody>
                    </table>
                </td>
            </tr>
        </tbody>
</table>  
      
#### Example

{% highlight html %}

    <ej-kanban id="kanban" [dataSource]="kanbanData" (toolbarClick)="onToolBarClick($event)"> 

{% endhighlight %}

{% highlight ts %}

    onToolBarClick(e: any){ 
         // Your code here
    }

{% endhighlight %}

