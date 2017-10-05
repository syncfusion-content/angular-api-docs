---
layout: post
title: Properties, Methods and Events of ejSchedule Widget
description: Methods, Members and Events available in ejSchedule
documentation: API
platform: angular-api
keywords: ejSchedule, API, Essential JS Schedule
---

# ejSchedule

An Event calendar that manages the list of various activities like events/appointments.

#### Syntax

{% highlight javascript %}

$(element).ejSchedule()

{% endhighlight %}

#### Example

{% highlight html %}

<ej-schedule id="Schedule"></ej-schedule>

{% endhighlight %}


#### Requires

* module:jQuery
* module:jquery.easing.min.js
* module:jsrender.min.js
* module:ej.globalize.min.js
* module:ej.core.js
* module:ej.data.js
* module:ej.scroller.js
* module:ej.touch.js
* module:ej.draggable.js
* module:ej.navigationdrawerbase.js
* module:ej.listviewbase.js
* module:ej.listview.js
* module:ej.radiobutton.js
* module:ej.editor.js
* module:ej.dropdownlist.js
* module:ej.autocomplete.js
* module:ej.menu.js
* module:ej.dialog.js
* module:ej.button.js
* module:ej.checkbox.js
* module:ej.datepicker.js
* module:ej.timepicker.js
* module:ej.navigationdrawer.js
* module:ej.recurrenceeditor.js
* module:ej.schedule.js

## Members

### allowDragAndDrop `boolean`
{:#members:allowdraganddrop}

When set to true, Schedule allows the appointments to be dragged and dropped at required time.

#### Default Value

* true

#### Example - To disable the drag and drop functionality.

{% highlight html %}

<ej-schedule id="Schedule" [currentDate]="CurrentDate" [allowDragAndDrop]="AllowDragAndDrop" [appointmentSettings.dataSource]="DataManager"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AllowDragAndDrop: boolean;
    public DataManager: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AllowDragAndDrop = false;
        this.DataManager = [{
            Id: 101,
            Subject: "Talk with Nature",
            StartTime: new Date(2014, 4, 5, 10, 00),
            EndTime: new Date(2014, 4, 5, 11, 00)
        }];
    }

}

{% endhighlight %}

### allowInline `boolean`
{:#members:allowinline}

When set to true, allows the user to create/edit appointments inline - simply through a single click made either on the Scheduler cells or on the existing appointment’s Subject text respectively. Pressing enter key after the new Subject text   typed onto the inline created text box, will save/update the appointments appropriately.

#### Default Value

* false

#### Example - To create/edit appointments through inline.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [allowInline]="AllowInline" [appointmentSettings.dataSource]="DataManager"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AllowInline: boolean;
    public DataManager: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AllowInline = true;
        this.DataManager = [{
            Id: 101,
            Subject: "Talk with Nature",
            StartTime: new Date(2014, 4, 5, 10, 00),
            EndTime: new Date(2014, 4, 5, 11, 00)
        }];
    }

}

{% endhighlight %}

## allowDelete `boolean`
{:#members:allowdelete}

When set to `false`, disables the appointment delete option on the Scheduler.

#### Default Value

* true

#### Example - To disable deletion of appointments from the scheduler.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [allowDelete]="AllowDelete" [appointmentSettings.dataSource]="DataManager"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AllowDelete: boolean;
    public DataManager: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AllowDelete = false;
        this.DataManager = [{
            Id: 101,
            Subject: "Talk with Nature",
            StartTime: new Date(2014, 4, 5, 10, 00),
            EndTime: new Date(2014, 4, 5, 11, 00)
        }];
    }

}

{% endhighlight %}

### allowKeyboardNavigation `boolean`
{:#members:allowkeyboardnavigation}

When set to true, Scheduler allows interaction through keyboard shortcut keys.

#### Default Value

* true

#### Example - To disable the Keyboard interaction with Schedule.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [allowKeyboardNavigation]="AllowKeyboardNavigation" [appointmentSettings.dataSource]="DataManager"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AllowKeyboardNavigation: boolean;
    public DataManager: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AllowKeyboardNavigation = false;
        this.DataManager = [{
            Id: 101,
            Subject: "Talk with Nature",
            StartTime: new Date(2014, 4, 5, 10, 00),
            EndTime: new Date(2014, 4, 5, 11, 00)
        }];
    }

}

{% endhighlight %}

### appointmentSettings `Object`
{:#members:appointmentsettings}

It includes the dataSource option and the fields related to Schedule appointments. The appointment fields within the appointmentSettings can accept both string and object type values. To apply validation rules on the appointment window fields, then the appointment fields needs to be defined with object type values.

#### Example – AppointmentSettings field mapped with string type values

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [appointmentSettings.dataSource]="DataManager" appointmentSettings.id="EventId" appointmentSettings.startTime="EventStartTime" appointmentSettings.endTime="EventEndTime"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public DataManager: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.DataManager = [{
            EventId: 101,
            EventStartTime: new Date(2014, 4, 5, 10, 00),
            EventEndTime: new Date(2014, 4, 5, 11, 00)
        }];
    }

}

{% endhighlight %}

#### Example – AppointmentSettings field mapped with object type

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                EventId: 101,
                EventSubject:"Play with pets",
                EventStartTime: new Date(2014, 4, 5, 10, 00),
                EventEndTime: new Date(2014, 4, 5, 12, 00),
                EventDescription:"Pet Lovers!!!"
            }],
            id: "EventId",
            subject: { field: "EventSubject", validationRules: { required: true } },
            startTime: { field: "EventStartTime", validationRules: { required: true } },
            endTime: { field: "EventEndTime", validationRules: { required: true } },
            description: { field: "EventDescription", validationRules: { required: true, minlength: 5, maxlength: 500 } },
        };
    }

}

{% endhighlight %}

### appointmentSettings.dataSource `Object|Array`
{:#members:appointmentsettings-datasource}

The dataSource option accepts either JSON object collection or DataManager ([ej.DataManager](/js/datamanager/overview)) instance that contains Schedule appointments.

#### Default Value

* []

#### Example - To set the dataSource with array of JSON object collection.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 12, 00)
            }, {
                Id: 102,
                Subject: "Play with pets",
                StartTime: new Date(2014, 4, 5, 05, 00),
                EndTime: new Date(2014, 4, 5, 07, 00)
            }]
        };
    }

}

{% endhighlight %}

#### Example - To set the dataSource with data manager instance.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: ej.DataManager({
                url: "http://mvc.syncfusion.com/OdataServices/Northwnd.svc/Events",
                crossDomain: true
            })
        };
    }

}

{% endhighlight %}

### appointmentSettings.query `string`
{:#members:appointmentsettings-query}

It holds either the ej.Query() object or simply the query string that retrieves the specified records from the table.

#### Default Value

* null

#### Example - Query the data manager to fetch specific record count from the Events table.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: ej.DataManager({
                url: "http://mvc.syncfusion.com/OdataServices/Northwnd.svc/Events",
                crossDomain: true
            }),
            query: ej.Query().from("Events").take(10)
        };
    }

}

{% endhighlight %}

### appointmentSettings.tableName `string`
{:#members:appointmentsettings-tablename}

Assign the table name from where the records are to be fetched for the Schedule.

#### Default Value

* null

#### Example - Using tableName property to fetch all the records directly from it.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: ej.DataManager({
                url: "http://mvc.syncfusion.com/OdataServices/Northwnd.svc",
                crossDomain: true
            }),
            tableName: "Events"
        };
    }

}

{% endhighlight %}

> The following are the appointment fields that holds the appropriate column names from the dataSource. All its default values are `null`.

### appointmentSettings.applyTimeOffset `boolean`
{:#members:appointmentsettings-applytimeoffset}

When set to false, doesn't consider the time difference offset calculation on appointment time.

#### Default Value

* true

#### Example - To set the timezone for schedule appointments or not.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            applyTimeOffset: false,
            dataSource: [{
                EventId: 101,
                EventStartTime: new Date(2014, 4, 5, 10, 00),
                EventEndTime: new Date(2014, 4, 5, 12, 00)
            }],
            id: "EventId",
            startTime: "EventStartTime",
            endTime: "EventEndTime"
        };
    }

}

{% endhighlight %}

### appointmentSettings.editFutureEventsOnly `boolean`
{:#members:appointmentsettings-editfutureeventsonly}

When set to true, introduces a new option to edit only the future occurrences of the appointments in a recurrence series from the currently selected appointment's date.

#### Default Value

* false

#### Example - To edit future appointments in recurrence series

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            editFutureEventsOnly: true,
            dataSource: [{
                EventId: 101,
                EventStartTime: new Date(2014, 4, 5, 10, 00),
                EventEndTime: new Date(2014, 4, 5, 12, 00)
            }],
            id: "EventId",
            startTime: "EventStartTime",
            endTime: "EventEndTime"
        };
    }

}

{% endhighlight %}

### appointmentSettings.id `string`
{:#members:appointmentsettings-id}

Binds the id field name in dataSource to the id of Schedule appointments. It denotes the unique id assigned to appointments.

#### Default Value

* null

### appointmentSettings.startTime `string`
{:#members:appointmentsettings-starttime}

Binds the name of startTime field in the dataSource with start time of the Schedule appointments. It indicates the date and Time when Schedule appointment actually starts.

#### Default Value

* null

### appointmentSettings.endTime `string`
{:#members:appointmentsettings-endtime}

Binds the name of endTime field in dataSource with the end time of Schedule appointments. It indicates the date and time when Schedule appointment actually ends.

#### Default Value

* null

#### Example - To create a simple appointment with the fields id, startTime and endTime.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                EventId: 101,
                EventStartTime: new Date(2014, 4, 5, 10, 00),
                EventEndTime: new Date(2014, 4, 5, 12, 00)
            }],
            id: "EventId",
            startTime: "EventStartTime",
            endTime: "EventEndTime"
        };
    }

}

{% endhighlight %}

> The fields startTime and endTime are mandatory fields to be specified to create an appointment.

### appointmentSettings.subject `string`
{:#members:appointmentsettings-subject}

Binds the name of subject field in the dataSource to appointment Subject. Indicates the Subject or title that gets displayed on Schedule appointments.

#### Default Value

* null

#### Example - To create an appointment with Subject.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                EventId: 101,
                EventStartTime: new Date(2014, 4, 5, 10, 00),
                EventEndTime: new Date(2014, 4, 5, 12, 00),
                EventSubject: "Play with pets"
            }],
            id: "EventId",
            startTime: "EventStartTime",
            endTime: "EventEndTime",
            subject: "EventSubject"
        };
    }

}

{% endhighlight %}

### appointmentSettings.description `string`
{:#members:appointmentsettings-description}

Binds the description field name in dataSource. It indicates the appointment description.

#### Default Value

* null

#### Example - To create an appointment with Description.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                EventId: 101,
                EventStartTime: new Date(2014, 4, 5, 10, 00),
                EventEndTime: new Date(2014, 4, 5, 12, 00),
                EventDescription: "Pet Lovers!!!"
            }],
            id: "EventId",
            startTime: "EventStartTime",
            endTime: "EventEndTime",
            description: "EventDescription"
        };
    }

}

{% endhighlight %}

> Unlike Subject field that gets displayed over an appointment with corresponding time, the description doesn’t show up on it, by default. To display description over appointments, the appointment template can be used.

### appointmentSettings.recurrence `string`
{:#members:appointmentsettings-recurrence}

Binds the name of recurrence field in dataSource. It indicates whether the appointment is a recurrence appointment or not.

#### Default Value

* null

### appointmentSettings.recurrenceRule `string`
{:#members:appointmentsettings-recurrencerule}

Binds the name of recurrenceRule field in dataSource. It indicates the recurrence pattern associated with appointments.

#### Default Value

* null

#### Example - To create a recurrence appointment.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                EventId: 101,
                EventSubject: "Play with Pets",
                EventStartTime: new Date(2014, 4, 5, 10, 00),
                EventEndTime: new Date(2014, 4, 5, 12, 00),
                EventRecurrence: true,
                EventRecurrenceRule: "FREQ=DAILY;INTERVAL=1;COUNT=10"
            }],
            id: "EventId",
            startTime: "EventStartTime",
            endTime: "EventEndTime",
            subject: "EventSubject",
            recurrence: "EventRecurrence",
            recurrenceRule: "EventRecurrenceRule"
        };
    }

}

{% endhighlight %}

> The recurrence and recurrenceRule fields are inter-dependent, as when the recurrence field is set to true, the recurrenceRule has to be defined mandatorily for an appointment.

### appointmentSettings.allDay `string`
{:#members:appointmentsettings-allday}

Binds the name of `allDay` field in dataSource. It indicates whether the appointment is an all-day appointment or not.

#### Default Value

* null

#### Example - To create an all-day appointment.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                EventId: 101,
                EventSubject: "Play with Pets",
                EventStartTime: new Date(2014, 4, 5, 10, 00),
                EventEndTime: new Date(2014, 4, 5, 12, 00),
                EventAllDay: true
            }],
            id: "EventId",
            startTime: "EventStartTime",
            endTime: "EventEndTime",
            subject: "EventSubject",
            allDay: "EventAllDay"
        };
    }

}

{% endhighlight %}

### appointmentSettings.resourceFields `string`
{:#members:appointmentsettings-resourcefields}

Binds one or more fields in resource collection dataSource. It maps the resource field names with appointments denoting the resource of appointments actually belongs.

#### Default Value

* null

#### Example - To create appointments in multiple resources scenario.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [group]="GroupData" [resources]="ResourceData" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public GroupData: any;
    public ResourceData: any;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.GroupData = {
            resources: ["Owners"]
        };
        this.ResourceData = [{
            field: "ownerId",
            title: "Owner",
            name: "Owners",
            allowMultiple: true,
            resourceSettings: {
                dataSource: [
                    { text: "Nancy", id: 1, color: "#f8a398" },
                    { text: "Steven", id: 2, color: "#56ca85"}
                ],
                text: "text", id: "id", color: "color"
            }
        }];
        this.AppointmentSettings = {
            dataSource: [{
                EventId: 100,
                EventSubject: "Research on Sky Miracles",
                EventStartTime: new Date(2014, 4, 2, 9, 00),
                EventEndTime: new Date(2014, 4, 2, 10, 30),
                ownerId: 2
            }],
            id: "EventId",
            startTime: "EventStartTime",
            endTime: "EventEndTime",
            subject: "EventSubject",
            resourceFields: "ownerId"
        };
    }

}

{% endhighlight %}

### appointmentSettings.categorize `string`
{:#members:appointmentsettings-categorize}

Binds the name of categorize field in dataSource. It indicates the categorize value, red categorize, green, yellow and so on applied to the appointments.

#### Default Value

* null

#### Example - To create appointments with categorize options.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [categorizeSettings]="CategorizeData" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public CategorizeData: any;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.CategorizeData = {
            enable: true
        };
        this.AppointmentSettings = {
            dataSource: [{
                EventId: 100,
                EventSubject: "Research on Sky Miracles",
                EventStartTime: new Date(2014, 4, 2, 9, 00),
                EventEndTime: new Date(2014, 4, 2, 10, 30),
                EventCategorize: "6"
            }],
            id: "EventId",
            startTime: "EventStartTime",
            endTime: "EventEndTime",
            subject: "EventSubject",
            categorize: "EventCategorize"
        };
    }

}

{% endhighlight %}

> There are six default Categorize colors available for appointments, Blue, Green, Orange, Purple, Red and Yellow that can be accessed by its default id values ranging from 1 to 6 respectively. The default Categorize collection can also be replaced with user-specified collection.


### appointmentSettings.location `string`
{:#members:appointmentsettings-location}

Binds the name of location field in dataSource. It indicates the appointment location.

#### Default Value

* null

#### Example - To create appointments with categorize options.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [showLocationField]="ShowLocationField" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public ShowLocationField: boolean;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.ShowLocationField = true;
        this.AppointmentSettings = {
            dataSource: [{
                EventId: 100,
                EventSubject: "Research on Sky Miracles",
                EventStartTime: new Date(2014, 4, 2, 9, 00),
                EventEndTime: new Date(2014, 4, 2, 10, 30),
                EventLocation: "Hawaii"
            }],
            id: "EventId",
            startTime: "EventStartTime",
            endTime: "EventEndTime",
            subject: "EventSubject",
            location: "EventLocation"
        };
    }

}

{% endhighlight %}

> To use the location field in Schedule, enable an additional API showLocationField that displays the location textbox on the default appointment window.

### appointmentSettings.priority `string`
{:#members:appointmentsettings-priority}

Binds the name of the priority field in dataSource. It indicates the priority, high, low, medium and none of the appointments.

#### Default Value

* null

#### Example - To create appointments with priority option.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [prioritySettings]="PriorityData" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public PriorityData: any;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.PriorityData = { enable:true };
        this.AppointmentSettings = {
            dataSource: [{
                EventId: 100,
                EventSubject: "Research on Sky Miracles",
                EventStartTime: new Date(2014, 4, 2, 9, 00),
                EventEndTime: new Date(2014, 4, 2, 10, 30),
                EventPriority: "high"
            }],
            id: "EventId",
            startTime: "EventStartTime",
            endTime: "EventEndTime",
            subject: "EventSubject",
            priority: "EventPriority"
        };
    }

}

{% endhighlight %}

> To use the priority field in Schedule, enable the prioritySettings that displays the priority textbox on the default appointment window.

### appointmentSettings.startTimeZone `string`
{:#members:appointmentsettings-starttimezone}

Binds the name of start timezone field in dataSource. It indicates the timezone of appointment start date. When startTimeZone field is not mentioned, the appointment uses the Schedule timeZone or System timeZone.

#### Default Value

* null

### appointmentSettings.endTimeZone `string`
{:#members:appointmentsettings-endtimezone}

Binds the name of end timezone field in dataSource. It indicates the timezone of appointment end date. When the endTimeZone field is not mentioned, the appointment uses the Schedule timeZone or System timeZone.

#### Default Value

* null

#### Example - To create appointments with StartTimeZone and EndTimeZone.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [prioritySettings]="PriorityData" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public PriorityData: any;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.PriorityData = { enable:true };
        this.AppointmentSettings = {
            dataSource: [{
                EventId: 100,
                EventSubject: "Research on Sky Miracles",
                EventStartTime: new Date(2014, 4, 2, 9, 00),
                EventEndTime: new Date(2014, 4, 2, 10, 30),
                EventStartTimeZone: "UTC +00:00",
                EventEndTimeZone: "UTC +00:00"
            }],
            id: "EventId",
            startTime: "EventStartTime",
            endTime: "EventEndTime",
            subject: "EventSubject",
            priority: "EventPriority",
            startTimeZone: "EventStartTimeZone",
            endTimeZone: "EventEndTimeZone"
        };
    }

}

{% endhighlight %}

### appointmentTemplateId `string`
{:#members:appointmenttemplateid}

Template design that applies on the Schedule appointments. All the field names that are mapped from dataSource to the appropriate field properties within the appointmentSettings can be used within the template.

#### Default Value

* null

#### Example - To set the appointment template.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" appointmentTemplateId="#appTemplate" [appointmentSettings]="AppointmentSettings"></ej-schedule>

<script id="appTemplate" type="text/x-jsrender">
   <div style="height:100%">
      <div>{{:Description}}</div>
   </div>
</script>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00),
                Description: "Splendid Nature!!!"
            }]
        };
    }

}

{% endhighlight %}

### cssClass `string`
{:#members:cssclass  }

Accepts the custom CSS class name that defines specific user-defined styles and themes to be applied for partial or complete elements of the Schedule.

#### Default Value

* ""

#### Example - To simply customize the background color of Scheduler header element by using custom CSS class name.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" cssClass="customStyle" [appointmentSettings]="AppointmentSettings"></ej-schedule>

<style type="text/css">
    .customStyle .e-scheduleheader {
        background-color: Teal;
    }
</style>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00),
                Description: "Splendid Nature!!!"
            }]
        };
    }

}

{% endhighlight %}

> For more information on applying custom themes to Syncfusion controls, refer [here](/js/theming-in-essential-javascript-components#customizing-themes).

### categorizeSettings `Object`
{:#members:categorizesettings}

Sets various categorize colors to the Schedule appointments to differentiate it.

### categorizeSettings.allowMultiple `boolean`
{:#members:categorizesettings-allowmultiple}

When set to true, enables the multiple selection of categories to be applied for the appointments.

#### Default Value

* false

#### Example - To enable multiple selection of categories.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [categorizeSettings]="CategorizeData" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public CategorizeData: any;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.CategorizeData = {
            enable: true,
            allowMultiple: true
        };
        this.AppointmentSettings = {
            dataSource: [{
                Id: 100,
                Subject: "Research on Sky Miracles",
                StartTime: new Date(2014, 4, 2, 9, 00),
                EndTime: new Date(2014, 4, 2, 10, 30),
                EventCategorize: "6,4,3"
            }],
            categorize: "EventCategorize"
        };
    }

}

{% endhighlight %}

### categorizeSettings.enable `boolean`
{:#members:categorizesettings-enable}

When set to true, enables the categories option to be applied for the appointments.

#### Default Value

* false

#### Example - To enable the categorize option.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [categorizeSettings]="CategorizeData" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public CategorizeData: any;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.CategorizeData = {
            enable: true
        };
        this.AppointmentSettings = {
            dataSource: [{
                Id: 100,
                Subject: "Research on Sky Miracles",
                StartTime: new Date(2014, 4, 2, 9, 00),
                EndTime: new Date(2014, 4, 2, 10, 30),
                EventCategorize: "6"
            }],
            categorize: "EventCategorize"
        };
    }

}

{% endhighlight %}

### categorizeSettings.dataSource `Array|Object`
{:#members:categorizesettings-datasource }

The dataSource option accepts either the JSON object collection or DataManager [[ej.DataManager](/js/datamanager/overview)] instance that contains the categorize data.

#### Default Value

*  {% highlight js %}
    [
       { text: "Blue Category", id: 1, color: "#43b496", fontColor: "#ffffff" },
       { text: "Green Category", id: 2, color: "#7f993e", fontColor: "#ffffff" },
       { text: "Orange Category", id: 3, color: "#cc8638", fontColor: "#ffffff" },
       { text: "Purple Category", id: 4, color: "#ab54a0", fontColor: "#ffffff" },
       { text: "Red Category", id: 5, color: "#dd654e", fontColor: "#ffffff" },
       { text: "Yellow Category", id: 6, color: "#d0af2b", fontColor: "#ffffff" }
    ]

   {% endhighlight %}

#### Example - To set the dataSource with array of JSON object collection.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [categorizeSettings]="CategorizeData" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public CategorizeData: any;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.CategorizeData = {
            enable: true,
            dataSource: [
                { text: "Good", id: 1, color: "#7499e1", fontColor: "red" },
                { text: "Excellent", id: 2, color: "#7cce6e", fontColor: "white" },
                { text: "Improve", id: 5, color: "#e04343", fontColor: "white" },
                { text: "Better", id: 6, color: "#f8f264", fontColor: "black"}
            ]
        };
        this.AppointmentSettings = {
            dataSource: [{
                Id: 100,
                Subject: "Research on Sky Miracles",
                StartTime: new Date(2014, 4, 2, 9, 00),
                EndTime: new Date(2014, 4, 2, 10, 30),
                EventCategorize: "6"
            }],
            categorize: "EventCategorize"
        };
    }

}

{% endhighlight %}

The following are the category fields that holds appropriate column names from dataSource.

### categorizeSettings.id `string`
{:#members:categorizesettings-id}

Binds id field name in the dataSource to id of category data.

#### Default Value

* "id"

### categorizeSettings.text `string`
{:#members:categorizesettings-text}

Binds text field name in the dataSource to category text.

#### Default Value

* "text"

### categorizeSettings.color `string`
{:#members:categorizesettings-color}

Binds color field name in the dataSource to category color.

#### Default Value

* "color"

#### Example - To set the categorize options with id, text and color fields.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [categorizeSettings]="CategorizeData" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public CategorizeData: any;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.CategorizeData = {
            enable: true,
            dataSource: [
                { CategoryText: "Good", Id: 1, CategoryColor: "#7499e1" },
                { CategoryText: "Excellent", Id: 2, CategoryColor: "#7cce6e" },
                { CategoryText: "Improve", Id: 5, CategoryColor: "#e04343" },
                { CategoryText: "Better", Id: 6, CategoryColor: "#f8f264" }
            ],
            text: "CategoryText",
            id: "Id",
            color: "CategoryColor"
        };
        this.AppointmentSettings = {
            dataSource: [{
                Id: 100,
                Subject: "Research on Sky Miracles",
                StartTime: new Date(2014, 4, 2, 9, 00),
                EndTime: new Date(2014, 4, 2, 10, 30),
                EventCategorize: "6"
            }],
            categorize: "EventCategorize"
        };
    }

}

{% endhighlight %}

### categorizeSettings.fontColor `string`
{:#members:categorizesettings-fontcolor}

Binds fontColor field name in the dataSource to category font.

#### Default Value

* "fontColor"

#### Example - To set categorize options with fontColor.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [categorizeSettings]="CategorizeData" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public CategorizeData: any;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.CategorizeData = {
            enable: true,
            dataSource: [
                { text: "Good", id: 1, color: "#7499e1", fontColor: "red" },
                { text: "Excellent", id: 2, color: "#7cce6e", fontColor: "red" }
            ]
        };
        this.AppointmentSettings = {
            dataSource: [{
                EventId: 100,
                EventSubject: "Research on Sky Miracles",
                EventStartTime: new Date(2014, 4, 2, 9, 00),
                EventEndTime: new Date(2014, 4, 2, 10, 30),
                EventCategorize: "2"
            }],
            id: "EventId",
            startTime: "EventStartTime",
            endTime: "EventEndTime",
            subject: "EventSubject",
            categorize: "EventCategorize"
        };
    }

}

{% endhighlight %}

### cellHeight `string`
{:#members:cellheight}

Sets the height for Schedule cells.

#### Default Value

* "20px"

#### Example - To set cell height for Scheduler.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" cellHeight="35px" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00)
            }]
        };
    }

}

{% endhighlight %}

### cellWidth `string`
{:#members:cellwidth}

Sets the width for Schedule cells.

#### Default Value

* ""

#### Example - To set the cell width for Schedule.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" cellWidth="180px" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00)
            }]
        };
    }

}

{% endhighlight %}

### contextMenuSettings `Object`
{:#members:contextmenusettings}

Holds all options related to the context menu settings of Scheduler.

### contextMenuSettings.enable `boolean`
{:#members:contextmenusettings-enable}

When set to true, enables the context menu options available for the Schedule cells and appointments.

#### Default Value

* false

#### Example - To enable the context menu options for Schedule control.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [contextMenuSettings]="ContextMenuData" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public ContextMenuData: any;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.ContextMenuData = {
            enable: true
        };
        this.AppointmentSettings = {
            dataSource: [{
                EventId: 100,
                EventSubject: "Research on Sky Miracles",
                EventStartTime: new Date(2014, 4, 2, 9, 00),
                EventEndTime: new Date(2014, 4, 2, 10, 30)
            }],
            id: "EventId",
            startTime: "EventStartTime",
            endTime: "EventEndTime",
            subject: "EventSubject"
        };
    }

}

{% endhighlight %}

### contextMenuSettings.menuItems `Object`
{:#members:contextmenusettings-menuitems}

Contains all the default context menu options that are applicable for both Schedule cells and appointments. It also supports adding custom menu items to cells or appointment collection.

### contextMenuSettings.menuItems.appointment `Array`
{:#members:contextmenusettings-menuitems-appointment}

All the appointment related context menu items are grouped under this appointment menu collection.

#### Default Value

* {% highlight js %}

    [
        { id: "open", text: "Open Appointment" },
        { id: "delete", text: "Delete Appointment" }
    ]

  {% endhighlight %}

### contextMenuSettings.menuItems.cells `Array`
{:#members:contextmenusettings-menuitems-cells}

All the Scheduler cell related context menu items are grouped under this cells menu item collection.

#### Default Value

* {% highlight js %}

    [
        { id: "new", text: "New Appointment" },
        { id: "recurrence", text: "New Recurring Appointment" },
        { id: "today", text: "Today" },
        { id: "gotoDate", text: "Go to date" },
        { id: "settings", text: "Settings" },
        { id: "view", text: "View", parentId: "settings" },
        { id: "timeMode", text: "TimeMode", parentId: "settings" },
        { id: "view_Day", text: "Day", parentId: "view" },
        { id: "view_Week", text: "Week", parentId: "view" },
        { id: "view_Workweek", text: "Workweek", parentId: "view" },
        { id: "view_Month", text: "Month", parentId: "view" },
        { id: "view_Agenda", text: "Agenda", parentId: "view" },
        { id: "timeMode_Hour12", text: "12 Hours", parentId: "timeMode" },
        { id: "timeMode_Hour24", text: "24 Hours", parentId: "timeMode" },
        { id: "workhours", text: "Work Hours", parentId: "settings" }
    ]

  {% endhighlight %}

#### Example - Default context menu options available for Schedule cells and appointments.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [contextMenuSettings]="ContextMenuData" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public ContextMenuData: any;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.ContextMenuData = {
            enable: true,
            menuItems: {
                appointment: [
                    { id: "open", text: "Open Appointment" },
                    { id: "delete", text: "Delete Appointment" }
                ],
                cells: [
                    { id: "new", text: "New Appointment" },
                    { id: "recurrence", text: "New Recurring Appointment" },
                    { id: "today", text: "Today" },
                    { id: "gotoDate", text: "Go to date" },
                    { id: "settings", text: "Settings" },
                    { id: "view", text: "View", parentId: "settings" },
                    { id: "timeMode", text: "TimeMode", parentId: "settings" },
                    { id: "view_Day", text: "Day", parentId: "view" },
                    { id: "view_Week", text: "Week", parentId: "view" },
                    { id: "view_Workweek", text: "Workweek", parentId: "view" },
                    { id: "view_Month", text: "Month", parentId: "view" },
                    { id: "timeMode_Hour12", text: "12 Hours", parentId: "timeMode" },
                    { id: "timeMode_Hour24", text: "24 Hours", parentId: "timeMode" },
                    { id: "workhours", text: "Work Hours", parentId: "settings" }
                ]
            }
        };
        this.AppointmentSettings = {
            dataSource: [{
                EventId: 100,
                EventSubject: "Research on Sky Miracles",
                EventStartTime: new Date(2014, 4, 2, 9, 00),
                EventEndTime: new Date(2014, 4, 2, 10, 30)
            }],
            id: "EventId",
            startTime: "EventStartTime",
            endTime: "EventEndTime",
            subject: "EventSubject"
        };
    }

}

{% endhighlight %}

#### Example - To add custom context menu option to the Schedule appointments.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [contextMenuSettings]="ContextMenuData" (menuItemClick)="onCustomMenuClick($event)" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public ContextMenuData: any;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.ContextMenuData = {
            enable: true,
            menuItems: {
                appointment: [
                    { id: "open", text: "Open Appointment" },
                    { id: "delete", text: "Delete Appointment" },
                    { id: "custom1", text: "Customize" }
                ],
                cells: [
                    { id: "new", text: "New Appointment" },
                    { id: "recurrence", text: "New Recurring Appointment" },
                    { id: "today", text: "Today" },
                    { id: "gotoDate", text: "Go to date" }
                ]
            }
        };
        this.AppointmentSettings = {
            dataSource: [{
                EventId: 100,
                EventSubject: "Research on Sky Miracles",
                EventStartTime: new Date(2014, 4, 2, 9, 00),
                EventEndTime: new Date(2014, 4, 2, 10, 30)
            }],
            id: "EventId",
            startTime: "EventStartTime",
            endTime: "EventEndTime",
            subject: "EventSubject"
        };
    }

    onCustomMenuClick(args) {
        if (args.events.ID == "custom1") {
            $("#Appointment_" + args.targetInfo.EventId).find(".e-apptext").html("Custom Appointment"); 
            $("#Appointment_" + args.targetInfo.EventId).css("background", "orange");
        }
    }

}

{% endhighlight %}

> In the above code example, `menuItemClick` event is defined that triggers when any of the menu options are selected. Here, the condition is checked as, when the id of selected menu item option contains *custom1*, then the target appointment’s text and its color gets modified.

### currentDate `Object`
{:#members:currentdate}

Sets current date of the Schedule. The Schedule displays initially with the date that is provided here.

#### Default Value

* new Date()

#### Example - To set current date for Scheduler.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00)
            }]
        };
    }

}

{% endhighlight %}

### currentView `string|enum`
{:#members:currentview}

<ts name="ej.Schedule.CurrentView"/>

Sets current view of the Schedule. Schedule renders initially with the view that is specified here. The available views are day, week, workweek, month, agenda and custom view - from which any one of the required view can be set to the Schedule. It accepts both string or enum values. The enum values that are accepted by currentView(ej.Schedule.CurrentView) are as follows,

<table class="params">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td class="name">Day</td>
            <td class="description">Sets currentView of the Scheduler as Day</td>
        </tr>
        <tr>
            <td class="name">Week</td>
            <td class="description">Sets currentView of the Scheduler as Week</td>
        </tr>
        <tr>
            <td class="name">Workweek</td>
            <td class="description">Sets currentView of the Scheduler as WorkWeek</td>
        </tr>
        <tr>
            <td class="name">Month</td>
            <td class="description">Sets currentView of the Scheduler as Month</td>
        </tr>
        <tr>
            <td class="name">Agenda</td>
            <td class="description">Sets currentView of the Scheduler as Agenda</td>
        </tr>
        <tr>
            <td class="name">CustomView</td>
            <td class="description">Sets currentView of the Scheduler as CustomView with user-specified date range.</td>
        </tr>
    </tbody>
</table>

#### Default Value

* ej.Schedule.CurrentView.Week

#### Example - To set the current view as Day for Schedule.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" currentView="day" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00)
            }]
        };
    }

}

{% endhighlight %}

### dateFormat `string`
{:#members:dateformat}

Sets the date format for Schedule.

#### Default Value

* ""

#### Example - To set the date format for Scheduler.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" dateFormat="yyyy-MM-dd" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00)
            }]
        };
    }

}

{% endhighlight %}

### showAppointmentNavigator `boolean`
{:#members:showappointmentnavigator}

When set to true, shows the previous/next appointment navigator button on the Scheduler.

#### Default Value

* true

#### Example - To hide the previous or next appointment navigator button.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [showAppointmentNavigator]="ShowAppointmentNavigator" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public ShowAppointmentNavigator: boolean;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.ShowAppointmentNavigator = false;
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00)
            }]
        };
    }

}

{% endhighlight %}

### enableAppointmentResize `boolean`
{:#members:enableappointmentresize}

When set to true, enables the resize behavior of appointments within the Schedule.

#### Default Value

* true

#### Example - To disable appointment resizing.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [enableAppointmentResize]="EnableAppointmentResize" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public EnableAppointmentResize: boolean;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.EnableAppointmentResize = false;
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00)
            }]
        };
    }

}

{% endhighlight %}

### enableLoadOnDemand `boolean`
{:#members:enableloadondemand}

When set to true, enables the loading of Schedule appointments based on your demand. With this load on demand concept, the data consumption of the Schedule can be limited.

#### Default Value

* false

#### Example - To enable the load on demand functionality for Schedule.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [enableLoadOnDemand]="EnableLoadOnDemand" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public EnableLoadOnDemand: boolean;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.EnableLoadOnDemand = true;
        this.AppointmentSettings = {
            dataSource: ej.DataManager({
                // To get the required appointments from service
                url: "http://mvc.syncfusion.com/OdataServices/api/ScheduleData/",
                crossDomain: true
            })
        };
    }

}

{% endhighlight %}

### enablePersistence `boolean`
{:#members:enablepersistence}

Saves the current model value to browser cookies for state maintenance. When the page gets refreshed, Schedule control values are retained.

#### Default Value

* false

#### Example - To enable persistence on Scheduler.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [enablePersistence]="EnablePersistence" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public EnablePersistence: boolean;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.EnablePersistence = true;
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00)
            }]
        };
    }

}

{% endhighlight %}

### enableRTL `boolean`
{:#members:enablertl}

When set to true, the Schedule layout and behavior changes as per the common RTL conventions.

#### Default Value

* false

#### Example - To enable RTL in Scheduler.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [enableRTL]="EnableRTL" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public EnableRTL: boolean;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.EnableRTL = true;
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00)
            }]
        };
    }

}

{% endhighlight %}

### endHour `number`
{:#members:endhour}

Sets the end hour time limit to be displayed on the Schedule.

#### Default Value

* 24

#### Example - To set end hour on the Scheduler.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [endHour]="EndHour" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public EndHour: number;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.EndHour = 18;
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00)
            }]
        };
    }

}

{% endhighlight %}

### group `Object`
{:#members:group}

To configure resource grouping on the Schedule.

> By default, group is assigned with null value.

### group.resources `Array`
{:#members:group-resources}

Holds the array of resource names to be grouped on the Schedule.

#### Example - To group the resources on Scheduler.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [group]="GroupData" [resources]="ResourceData" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public GroupData: any;
    public ResourceData: any;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.GroupData = {
            resources: ["Owners"]
        };
        this.ResourceData = [{
            field: "ResourceId",
            title: "Resource",
            name: "Owners",
            allowMultiple: true,
            resourceSettings: {
                dataSource: [
                    { text: "Nancy", id: 1, groupId: 1, color: "#f8a398" },
                    { text: "Steven", id: 3, groupId: 2, color: "#56ca85" },
                    { text: "Michael", id: 5, groupId: 1, color: "#51a0ed" }
                ],
                text: "text", id: "id", groupId: "groupId", color: "color"
            }
        }];
        this.AppointmentSettings = {
            resourceFields: "ResourceId",
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00),
                ResourceId: 3
            }]
        };
    }

}

{% endhighlight %}

### height `string`
{:#members:height}

Sets the height of the Schedule. Accepts both pixel and percentage values.

#### Default Value

* "1120px"

#### Example - To set the height of Scheduler in pixels.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" height="500px" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00)
            }]
        };
    }

}

{% endhighlight %}

#### Example - To set height of Scheduler in percentage.

> To set the percentage values for the Schedule height, define the parent element with some specific height that holds the Scheduler div. When the Schedule is not placed within any of the parent element, define the HTML and body tags explicitly with some height values either in pixel or percentage.

{% highlight html %}

<!DOCTYPE html>
<html xmlns="http://www.w3.org/1999/xhtml" style="height:100%">
<head>
    <!--[CSS and SCRIPT reference section]-->
</head>

<body style="height:100%">

<ej-schedule id="Schedule" width="100%" height="100%" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings"></ej-schedule>

</body>
</html>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00)
            }]
        };
    }

}

{% endhighlight %}

### workHours `Object`
{:#members:workhours}

To define the work hours within the Schedule control.

### workHours.highlight `boolean`
{:#members:workhours-hightlight}

When set to true, highlights the work hours of the Schedule.

#### Default Value

* true

#### Example - To disable the highlighting of Schedule work hours.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [workHours.highlight]="HighlightWorkHours" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public HighlightWorkHours: boolean;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.HighlightWorkHours = false;
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00)
            }]
        };
    }

}

{% endhighlight %}

### workHours.start `number`
{:#members:workhours-start}

Sets the start time to depict the start of working or business hour in a day.

#### Default Value

* 9

#### Example - To set the working start hour for Scheduler.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [workHours]="WorkHours" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public WorkHours: any;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.WorkHours = {
            highlight: false,
            start: 7
        };
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00)
            }]
        };
    }

}

{% endhighlight %}

### workHours.end `number`
{:#members:workhours-end}

Sets the end time to depict the end of working or business hour in a day.

#### Default Value

* 18

#### Example - To set the working end hour for Scheduler.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [workHours]="WorkHours" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public WorkHours: any;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.WorkHours = {
            highlight: false,
            start: 9,
            end: 20
        };
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00)
            }]
        };
    }

}

{% endhighlight %}

### isDST `boolean`
{:#members:isdst}

When set to true, enables the Schedule to observe Daylight Saving Time for supported timezones.

#### Default Value

* false

#### Example - To enable the Daylight Saving time in Schedule.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [isDST]="IsDST" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public IsDST: boolean;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.IsDST = true;
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00)
            }]
        };
    }

}

{% endhighlight %}

### isResponsive `boolean`
{:#members:isresponsive}

When set to true, adapts the Schedule layout to fit the screen size of devices on which it renders.

#### Default Value

* true

#### Example - To make the Scheduler adaptive.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [isResponsive]="Responsive" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public Responsive: boolean;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.Responsive = true;
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00)
            }]
        };
    }

}

{% endhighlight %}

### locale `string`
{:#members:locale}

Sets the specific culture to the Schedule.

#### Default Value

* "en-US"

#### Example - To set the French culture on Schedule, set its locale as fr-FR.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" locale="fr-FR" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00)
            }]
        };
    }

}

{% endhighlight %}

> To set any culture for Schedule, refer to the required minified globalize files of the specific culture. For example, to use fr-FR culture in Schedule, refer to the **globalize.culture.fr-FR.min.js** script file. Also define the locale words of that specific culture properly. For example, define the locale words for fr-FR culture in a variable ej.Schedule.Locale[“fr-FR”] = { }; under script section.

### maxDate `Object`
{:#members:maxdate}

Sets the maximum date limit to display on the Schedule. Setting maxDate with specific date value disallows the Schedule to navigate beyond that date.

#### Default Value

* new Date(2099, 12, 31)

#### Example - To set the maximum date on the Scheduler.


{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [maxDate]="MaxDate" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public MaxDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.MaxDate = new Date(2014, 4, 6);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00)
            }]
        };
    }

}

{% endhighlight %}

### minDate `Object`
{:#members:mindate}

Sets the minimum date limit to display on the Schedule. Setting minDate with specific date value disallows the Schedule to navigate beyond that date.

#### Default Value
{:.param}

* new Date(1900, 01, 01)

#### Example - To set the minimum date on the Scheduler.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [minDate]="MinDate" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public MinDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.MinDate = new Date(2014, 4, 3);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00)
            }]
        };
    }

}

{% endhighlight %}

### orientation `string|enum`
{:#members:orientation}

<ts name="ej.Schedule.Orientation"/>

Sets the mode of Schedule rendering either in a vertical or horizontal direction. It accepts either string("vertical" or "horizontal") or enum values. The enum values that are accepted by orientation(ej.Schedule.Orientation) are as follows,

<table class="params">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td class="name">Vertical</td>
            <td class="description">Set orientation as vertical to Scheduler</td>
        </tr>
        <tr>
            <td class="name">Horizontal</td>
            <td class="description">Set orientation as horizontal to Scheduler</td>
        </tr>
    </tbody>
</table>

#### Default Value

* ej.Schedule.Orientation.Vertical

#### Example - To render the Scheduler in horizontal orientation.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" orientation="horizontal" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00)
            }]
        };
    }

}

{% endhighlight %}

### prioritySettings `Object`
{:#members:prioritysettings}

Holds all the options related to priority settings of the Schedule.

### prioritySettings.enable `boolean`
{:#members:prioritysettings-enable}

When set to true, enables the priority options available for the Schedule appointments.

#### Default Value

* false

#### Example - To enable the priority option in Schedule.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [prioritySettings]="PriorityData" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public PriorityData: any;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.PriorityData = { enable: true };
        this.AppointmentSettings = {
            priority: "Priority",
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00),
                Priority: "high"
            }]
        };
    }

}

{% endhighlight %}

### prioritySettings.dataSource `Object|Array`
{:#members:prioritysettings-datasource }

The dataSource option can accept the JSON object collection that contains the priority related data.

#### Default Value

* {% highlight js%}
    [
        { text: "None", value: "none" },
        { text: "High", value: "high" },
        { text: "Medium", value: "medium" },
        { text: "Low", value: "low" }
    ]
  {% endhighlight %}

#### Example - To set the dataSource with array of JSON object collection.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [prioritySettings]="PriorityData" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public PriorityData: any;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.PriorityData = {
            enable: true,
            dataSource: [
                { text: "None", value: "none" },
                { text: "High", value: "high" },
                { text: "Medium", value: "medium" },
                { text: "Low", value: "low" }
            ]
        };
        this.AppointmentSettings = {
            dataSource: [{
                Id: 100,
                Subject: "Research on Sky Miracles",
                StartTime: new Date(2014, 4, 2, 9, 00),
                EndTime: new Date(2014, 4, 2, 10, 30),
                EventPriority: "low"
            }],
            priority: "EventPriority"
        };
    }

}

{% endhighlight %}

> The following are the priority fields that holds the appropriate column names from dataSource.

### prioritySettings.text `string`
{:#members:prioritysettings-text }

Binds text field name in the dataSource to prioritySettings text. These text gets listed out in priority field of the appointment window.

#### Default Value

* "text"

### prioritySettings.value `string`
{:#members:prioritysettings-value }

Binds value field name in the dataSource to prioritySettings value. These field names usually accepts four priority values by default, high, low, medium and none.

#### Default Value

* "value"

#### Example - To set the priority options with text and value fields.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [prioritySettings]="PriorityData" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public PriorityData: any;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.PriorityData = {
            enable: true,
            dataSource: [
                { PriorityText: "None", PriorityValue: "none" },
                { PriorityText: "Important", PriorityValue: "high" },
                { PriorityText: "Normal", PriorityValue: "medium" },
                { PriorityText: "Least", PriorityValue: "low" }
            ],
            text: "PriorityText",
            value: "PriorityValue"
        };
        this.AppointmentSettings = {
            dataSource: [{
                Id: 100,
                Subject: "Research on Sky Miracles",
                StartTime: new Date(2014, 4, 2, 9, 00),
                EndTime: new Date(2014, 4, 2, 10, 30),
                EventPriority: "low"
            }],
            priority: "EventPriority"
        };
    }

}

{% endhighlight %}

### prioritySettings.template `string`
{:#members:prioritysettings-template}

Allows priority field customization in the appointment window to add custom icons denoting the priority level for the appointments.

#### Default Value

* null

#### Example - To set the template for priority option in Schedule.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [prioritySettings]="PriorityData" [appointmentSettings]="AppointmentSettings"></ej-schedule>

<style type="text/css">
    .high,
    .medium {
        height: 13px;
        width: 13px;
        float: left;
        margin-right: 4px;
        background-repeat: no-repeat;
        background-size: 60px;
        padding: 1px;
        margin-top: 2px;
    }

    .high {
        /*background: url('Content/ej/web/images/critical.png');*/
        background-color: orange;
        background-position: -13px;
    }

    .medium {
        /*background: url('Content/ej/web/images/ultracritical.png');*/
        background-color: #56ca85;
        background-position: -59px;
    }
</style>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public PriorityData: any;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.PriorityData = {
            enable: true,
            dataSource: [
                { text: "High", value: "high" },
                { text: "Normal", value: "medium" }
            ],
            text: "text", value: "value",
            template: "<div class='${value}'></div>"
        };
        this.AppointmentSettings = {
            priority: "Priority",
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00),
                Priority: "high"
            }]
        };
    }

}

{% endhighlight %}

> Since the `prioritySettings` contains the default values in its dataSource like none, high, medium and low, the appropriate CSS classes has to be created with the same value names to apply it on the template.

### readOnly `boolean`
{:#members:readonly }

When set to true, disables the interaction with the Schedule appointments, simply allowing the date and view navigation to occur.

#### Default Value

* false

#### Example - To make the Scheduler readOnly.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [readOnly]="ReadOnly" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public ReadOnly: boolean;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.ReadOnly = true;
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00)
            }]
        };
    }

}

{% endhighlight %}

### reminderSettings `Object`
{:#members:remindersettings }

Holds all the options related to reminder settings of the Schedule.

### reminderSettings.enable `boolean`
{:#members:remindersettings-enable }

When set to true, enables the reminder option available for the Schedule appointments.

#### Default Value

* false

#### Example - To enable the reminder option in Scheduler.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [reminderSettings]="ReminderData" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public ReminderData: any;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.ReminderData = { enable: true };
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00)
            }]
        };
    }

}

{% endhighlight %}

### reminderSettings.alertBefore `number`
{:#members:remindersettings-alertbefore}

Sets the timing, when the reminders are to be alerted for the Schedule appointments.

#### Default Value

* 5

#### Example - To set the alert for Schedule appointments.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [reminderSettings]="ReminderData" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public ReminderData: any;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.ReminderData = {
            enable: true,
            alertBefore: 7
        };
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00)
            }]
        };
    }

}

{% endhighlight %}

### renderDates `Object`
{:#members:renderdates}

Defines the specific start and end dates to be rendered in the Schedule control. To render such user-specified custom date ranges in the Schedule control, set the **currentView** property to `ej.Schedule.CurrentView.CustomView`.

#### Default Value

* null

### renderDates.start `Object`
{:#members:renderdates-start}

Sets the start of custom date range to be rendered in the Schedule.

#### Default Value

* null

### renderDates.end `Object`
{:#members:renderdates-end}

Sets the end limit of the custom date range.

#### Default Value

* null

#### Example - To set the custom date range in Scheduler.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [views]="ViewData" currentView="customview" [renderDates]="RenderDates" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public ViewData: any;
    public RenderDates: any;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.ViewData = ["Day", "Week", "WorkWeek", "Month", "CustomView"];
        this.RenderDates = {
            start: new Date(2014, 11, 7),
            end: new Date(2014, 12, 10)
        };
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00)
            }]
        };
    }

}

{% endhighlight %}

### resourceHeaderTemplateId `string`
{:#members:resourceheadertemplateid}

Template design that applies on the Schedule resource header.

All field names that are mapped from the dataSource to appropriate field properties within the resourceSettings can be used within the template.

#### Default Value

* null

#### Example - To set the resource header template.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" resourceHeaderTemplateId="#resTemplate" [group]="GroupData" [resources]="ResourceData" [appointmentSettings]="AppointmentSettings"></ej-schedule>

<script id="resTemplate" type="text/x-jsrender">
<div style="height:100%">
    <div style="width:15px;height:15px;margin-left:25px;margin-top:3px;float:left;background:{{:color}};"></div>
    <div>{{:text}}</div>
</div>
</script>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public GroupData: any;
    public ResourceData: any;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.GroupData = {
            resources: ["Rooms"]
        };
        this.ResourceData = [{
            field: "roomId",
            title: "Room",
            name: "Rooms",
            allowMultiple: false,
            resourceSettings: {
                dataSource: [
                    { text: "ROOM1", id: 1, color: "#cb6bb2" },
                    { text: "ROOM2", id: 2, color: "#56ca85"}
                ],
                text: "text", id: "id", color: "color"
            }
        }];
        this.AppointmentSettings = {
            resourceFields: "roomId",
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00),
                roomId: 2
            }]
        };
    }

}

{% endhighlight %}

### resources `Array`
{:#members:resources}

Holds all the options related to the resources settings of the Schedule. It is a collection of one or more resource objects, where the levels of resources are rendered on the Schedule based on the order of the resource data provided within this collection.

#### Default Value

* null

### resources.field `string`
{:#members:resources-fields}

It holds the name of the resource field to be bound to the Schedule appointments that contains the resource Id.

#### Default Value

* null

#### Example - To specify the resource field.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [resources]="ResourceData" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public ResourceData: any;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.ResourceData = [{
            field: "ownerId",
            title: "Owner",
            resourceSettings: {
                dataSource: [
                    { text: "Nancy", id: 1, color: "#f8a398" },
                    { text: "Steven", id: 2, color: "#56ca85"}
                ],
                text: "text", id: "id", color: "color"
            }
        }];
        this.AppointmentSettings = {
            dataSource: [{
                Id: 100,
                Subject: "Research on Sky Miracles",
                StartTime: new Date(2014, 04, 05, 9, 00),
                EndTime: new Date(2014, 04, 05, 10, 30),
                ownerId: 2
            }],
            // bind one or more resources fields separated by commas
            resourceFields: "ownerId"
        };
    }

}

{% endhighlight %}

### resources.title `string`
{:#members:resources-title}

It holds the title name of the resource field to be displayed on the Schedule appointment window.

#### Default Value

* null

#### Example - To specify the resource title.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [resources]="ResourceData" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public ResourceData: any;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.ResourceData = [{
            field: "ownerId",
            title: "Owner",
            resourceSettings: {
                dataSource: [
                    { text: "Nancy", id: 1, color: "#f8a398" },
                    { text: "Steven", id: 2, color: "#56ca85"}
                ],
                text: "text", id: "id", color: "color"
            }
        }];
        this.AppointmentSettings = {
            dataSource: [{
                Id: 100,
                Subject: "Research on Sky Miracles",
                StartTime: new Date(2014, 04, 05, 9, 00),
                EndTime: new Date(2014, 04, 05, 10, 30),
                ownerId: 2
            }],
            resourceFields: "ownerId"
        };
    }

}

{% endhighlight %}

### resources.name `string`
{:#members:resources-name}

A unique resource name that is used for differentiating various resource objects while grouping it in various levels.

#### Default Value

* null

#### Example - To specify the resource name field.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [group]="GroupData" [resources]="ResourceData" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public GroupData: any;
    public ResourceData: any;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.GroupData = {
            resources: ["Owners"]
        };
        this.ResourceData = [{
            field: "ownerId",
            title: "Owner",
            name: "Owners",
            resourceSettings: {
                dataSource: [
                    { text: "Nancy", id: 1, color: "#f8a398" },
                    { text: "Steven", id: 2, color: "#56ca85"}
                ],
                text: "text", id: "id", color: "color"
            }
        }];
        this.AppointmentSettings = {
            dataSource: [{
                Id: 100,
                Subject: "Research on Sky Miracles",
                StartTime: new Date(2014, 04, 05, 9, 00),
                EndTime: new Date(2014, 04, 05, 10, 30),
                ownerId: 2
            }],
            // bind one or more resources fields separated by commas
            resourceFields: "ownerId"
        };
    }

}

{% endhighlight %}

### resources.allowMultiple `boolean`
{:#members:resources-allowmultiple}

When set to true, allows multiple selection of resource names, thus creating multiple instances of same appointment for the selected resources.

#### Default Value

* false

#### Example - To set allowMultiple option for a resource object.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [resources]="ResourceData" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public ResourceData: any;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.ResourceData = [{
            field: "ownerId",
            title: "Owner",
            resourceSettings: {
                dataSource: [
                    { text: "Nancy", id: 1, color: "#f8a398" },
                    { text: "Steven", id: 2, color: "#56ca95"}
                ],
                text: "text", id: "id", color: "color"
            }
        }, {
            field: "roomId",
            title: "Room(s)",
            allowMultiple: true,
            resourceSettings: {
                dataSource: [
                    { text: "Room1", id: 1, groupId: 1, color: "#f8a398" },
                    { text: "Room2", id: 2, groupId: 2, color: "#56ca85"},
                    { text: "Room3", id: 3, groupId: 2, color: "#56ac88"}
                ],
                text: "text", id: "id", color: "color", groupId: "groupId"
            }
        }];
        this.AppointmentSettings = {
            dataSource: [{
                Id: 100,
                Subject: "Research on Sky Miracles",
                StartTime: new Date(2014, 04, 05, 9, 00),
                EndTime: new Date(2014, 04, 05, 10, 30),
                ownerId: 2,
                roomId: 3
            }],
            resourceFields: "ownerId,roomId"
        };
    }

}

{% endhighlight %}

### resources.resourceSettings `Object`
{:#members:resources-resourcesettings}

It holds the field names of the resources to be bound to the Schedule and also the dataSource.

### resources.resourceSettings.dataSource `Object|Array`
{:#members:resources-resourcesettings-datasource}

The dataSource option accepts either JSON object collection or DataManager ([ejDataManager](/js/datamanager/overview)) instance that contains the resources related data.

#### Default Value

* []

#### Example - To set the dataSource with array of JSON object collection.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [resources]="ResourceData" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public ResourceData: any;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.ResourceData = [{
            field: "ownerId",
            title: "Owner",
            resourceSettings: {
                dataSource: [
                    { text: "Nancy", id: 1, color: "#f8a398" },
                    { text: "Steven", id: 2, color: "#56ca85"}
                ],
                text: "text", id: "id", color: "color"
            }
        }];
        this.AppointmentSettings = {
            dataSource: [{
                Id: 100,
                Subject: "Research on Sky Miracles",
                StartTime: new Date(2014, 04, 05, 9, 00),
                EndTime: new Date(2014, 04, 05, 10, 30),
                ownerId: 2
            }],
            resourceFields: "ownerId"
        };
    }

}

{% endhighlight %}

The following are the `resourceSettings` fields, that maps the appropriate column names from the dataSource.

### resources.resourceSettings.text `string`
{:#members:resources-resourcesettings-text}

Binds text field name in the dataSource to resourceSettings **text**. These text gets listed out in resources field of the appointment window.

#### Default Value

* null

### resources.resourceSettings.id `string`
{:#members:resources-resourcesettings-id}

Binds id field name in the dataSource to resourceSettings **id**.

#### Default Value

* null

### resources.resourceSettings.groupId `string`
{:#members:resources-resourcesettings-groupid}

Binds groupId field name in the dataSource to resourceSettings **groupId**.

#### Default Value

* null

### resources.resourceSettings.color `string`
{:#members:resources-resourcesettings-color}

Binds color field name in the dataSource to resourceSettings **color**. The color specified here gets applied to the Schedule appointments denoting to the resource it belongs.

#### Default Value

* null

### resources.resourceSettings.start `string`
{:#members:resources-resourcesettings-start}

Binds the starting work hour field name in the dataSource. It's optional, but providing it with some numeric value will set the starting work hour for specific resources.

#### Default Value

* null

### resources.resourceSettings.end `string`
{:#members:resources-resourcesettings-end}

Binds the end work hour field name in the dataSource. It's optional, but providing it with some numeric value will set the end work hour for specific resources.

#### Default Value

* null

### resources.resourceSettings.workWeek `string`
{:#members:resources-resourcesettings-workweek}

Binds the resources working days field name in the dataSource. It's optional, and accepts the array of strings (week day names). When provided with specific collection of days (array of day names), only those days will render for the specific resources.

#### Default Value

* null

#### Example - To set the resources options with id, text, groupId, color, start, end and workWeek fields.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [resources]="ResourceData" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public ResourceData: any;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.ResourceData = [{
            field: "ownerId",
            title: "Owner",
            resourceSettings: {
                dataSource: [
                    { OwnerText: "Nancy", id: 1, OwnerColor: "#f8a398" },
                    { OwnerText: "Steven", id: 2, OwnerColor: "#56ca95"}
                ],
                text: "OwnerText", id: "id", color: "OwnerColor"
            }
        }, {
            field: "roomId",
            title: "Room(s)",
            resourceSettings: {
                dataSource: [
                    // groupId groups the current resources under the previous level of resource object
                    { text: "Room1", id: 1, groupId: 1, color: "#f8a398", start: "10", end: "15", workWeek: ["monday","wednesday","friday"] },
                    { text: "Room2", id: 2, groupId: 2, color: "#56ca85", start: "10", end: "15", workWeek: ["tuesday","thursday"] },
                    { text: "Room3", id: 3, groupId: 2, color: "#56ac88", start: "10", end: "15", workWeek: ["sunday","saturday"] }
                ],
                text: "text", id: "id", color: "color", groupId: "groupId", start: "start", end: "end", workWeek: "workWeek"
            }
        }];
        this.AppointmentSettings = {
            dataSource: [{
                Id: 100,
                Subject: "Research on Sky Miracles",
                StartTime: new Date(2014, 04, 05, 9, 00),
                EndTime: new Date(2014, 04, 05, 10, 30),
                ownerId: 2,
                roomId: 3
            }],
            resourceFields: "ownerId,roomId"
        };
    }

}

{% endhighlight %}

### resources.resourceSettings.appointmentClass `string`
{:#members:resources-resourcesettings-appointmentclass}

Binds appointmentClass field name in the dataSource. It applies custom CSS class name to appointments depicting to the resource it belongs.

#### Default Value

* null

#### Example - To customize the styles of the appointments based on the resources it belongs, use the appointmentClass field with other resources options.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [resources]="ResourceData" [appointmentSettings]="AppointmentSettings"></ej-schedule>

<style type="text/css">
    .e-schedule .e-appointcss1 {
        background-color: Maroon;
        color: Orange;
    }
    .e-schedule .e-appointcss2 {
        background-color: Orange;
        color: Maroon;
    }
</style>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public ResourceData: any;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.ResourceData = [{
            field: "ownerId",
            title: "Owner",
            resourceSettings: {
                dataSource: [
                    { OwnerText: "Nancy", id: 1, customClass: "e-appointcss1" },
                    { OwnerText: "Steven", id: 2, customClass: "e-appointcss2"}
                ],
                text: "OwnerText", id: "id", appointmentClass: "customClass"
            }
        }];
        this.AppointmentSettings = {
            dataSource: [{
                Id: 100,
                Subject: "Research on Sky Miracles",
                StartTime: new Date(2014, 04, 05, 9, 00),
                EndTime: new Date(2014, 04, 05, 10, 30),
                ownerId: 2
            }, {
                Id: 101,
                Subject: "Discovery of exoplanets",
                StartTime: new Date(2014, 04, 07, 6, 00),
                EndTime: new Date(2014, 04, 07, 9, 30),
                ownerId: 1
            }],
            resourceFields: "ownerId"
        };
    }

}

{% endhighlight %}

> The custom CSS class names defined separately for each resources within 'style' tag are prefixed with the class name '.e-schedule', only then it gets applied to the appointments.

### showAllDayRow `boolean`
{:#members:showalldayrow}

When set to true, displays the all-day row cells on the Schedule.

#### Default Value

* true

#### Example - To hide the all-day row cells.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [showAllDayRow]="ShowAllDayRow" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public ShowAllDayRow: boolean;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.ShowAllDayRow = false;
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00)
            }]
        };
    }

}

{% endhighlight %}

### showWeekend `boolean`
{:#members:showweekend}

When set to `false`, hides the weekend days on all the Scheduler views.

#### Default Value

* true

#### Example - To hide the weekend days.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [showWeekend]="ShowWeekend" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public ShowWeekend: boolean;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.ShowWeekend = false;
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00)
            }]
        };
    }

}

{% endhighlight %}

### showCurrentTimeIndicator `boolean`
{:#members:showcurrenttimeindicator}

When set to true, displays the current time indicator on the Schedule.

#### Default Value

* true

#### Example - To hide the current time indicator.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [showCurrentTimeIndicator]="ShowCurrentTimeIndicator" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public ShowCurrentTimeIndicator: boolean;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.ShowCurrentTimeIndicator = false;
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00)
            }]
        };
    }

}

{% endhighlight %}

### showHeaderBar `boolean`
{:#members:showheaderbar}

When set to true, displays the header bar on the Schedule.

#### Default Value

* true

#### Example - To hide the Schedule header bar.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [showHeaderBar]="ShowHeaderBar" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public ShowHeaderBar: boolean;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.ShowHeaderBar = false;
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00)
            }]
        };
    }

}

{% endhighlight %}

### showLocationField `boolean`
{:#members:showlocationfield}

When set to true, displays the location field additionally on Schedule appointment window.

#### Default Value

* false

#### Example - To show the location field.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [showLocationField]="ShowLocationField" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public ShowLocationField: boolean;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.ShowLocationField = true;
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00),
                Location: "Chicago"
            }],
            location: "Location"
        };
    }

}

{% endhighlight %}

### showTimeZoneFields `boolean`
{:#members:showtimezonefields}

When set to false, doesn't render the start and end timezone fields on the Schedule appointment window.

#### Default Value

* true

#### Example - To show or hide the timezone field in appointment window.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [showTimeZoneFields]="ShowTimeZoneFields" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public ShowTimeZoneFields: boolean;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.ShowTimeZoneFields = false;
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00),
                Location: "Chicago"
            }],
            location: "Location"
        };
    }

}

{% endhighlight %}

### showQuickWindow `boolean`
{:#members:showquickwindow}

When set to true, displays the quick window for every single click made on the Schedule cells or appointments.

#### Default Value

* true

#### Example - To hide the quick window.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [showQuickWindow]="ShowQuickWindow" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public ShowQuickWindow: boolean;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.ShowQuickWindow = false;
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00)
            }]
        };
    }

}

{% endhighlight %}

### startHour `number`
{:#members:starthour}

Sets the start hour time range to be displayed on the Schedule.

#### Default Value

* 0

#### Example - To set the start hour on the Scheduler.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [startHour]="StartHour" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public StartHour: number;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.StartHour = 9;
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00)
            }]
        };
    }

}

{% endhighlight %}

### timeMode `string|enum`
{:#members:timemode}

<ts name="ej.Schedule.TimeMode"/>

Sets either 12 or 24 hour time mode on the Schedule. It accepts either the string value("12" or "24") or the below mentioned enum values. The enum values that are accepted by timeMode(ej.Schedule.TimeMode) are as follows,

<table class="params">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td class="name">Hour12</td>
            <td class="description">Sets 12 hour time mode to Scheduler</td>
        </tr>
        <tr>
            <td class="name">Hour24</td>
            <td class="description">Sets 24 hour time mode to Scheduler</td>
        </tr>
    </tbody>
</table>

#### Default Value

* null

#### Example - To set the 24 hour time mode on the Scheduler.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" timeMode="24" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00)
            }]
        };
    }

}

{% endhighlight %}

### timeZone `string`
{:#members:timezone}

Sets the timezone for the Schedule.

#### Default Value

* null

#### Example - To set the timezone in Scheduler.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" timeZone="UTC +2:00" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00)
            }]
        };
    }

}

{% endhighlight %}

### timeZoneCollection `Object`
{:#members:timezonecollection}

Sets the collection of timezone items to be bound to the Schedule. Only the items bound to this property gets listed out in the timezone field of the appointment window.

### timeZoneCollection.dataSource `Object`
{:#members:timezonecollection-datasource}

Sets the collection of timezone items to the dataSource that accepts either JSON object collection or DataManager ([ej.DataManager](https://help.syncfusion.com/js/datamanager/overview)) instance that contains Schedule timezones.

#### Default Value

* {% highlight js %}

    [
        { text: "UTC -12:00", id: "1", value: "UTC -12:00" },
        { text: "UTC -11:00", id: "2", value: "UTC -11:00" },
        { text: "UTC -10:00", id: "3", value: "UTC -10:00" },
        { text: "UTC -09:00", id: "4", value: "UTC -09:00" },
        { text: "UTC -08:00", id: "5", value: "UTC -08:00" },
        { text: "UTC -07:00", id: "6", value: "UTC -07:00" },
        { text: "UTC -06:00", id: "7", value: "UTC -06:00" },
        { text: "UTC -05:00", id: "8", value: "UTC -05:00" },
        { text: "UTC -04:30", id: "9", value: "UTC -04:30" },
        { text: "UTC -04:00", id: "10", value: "UTC -04:00" },
        { text: "UTC -03:30", id: "11", value: "UTC -03:30" },
        { text: "UTC -03:00", id: "12", value: "UTC -03:00" },
        { text: "UTC -02:00", id: "13", value: "UTC -02:00" },
        { text: "UTC -01:00", id: "14", value: "UTC -01:00" },
        { text: "UTC +00:00", id: "15", value: "UTC +00:00" },
        { text: "UTC +01:00", id: "16", value: "UTC +01:00" },
        { text: "UTC +02:00", id: "17", value: "UTC +02:00" },
        { text: "UTC +03:00", id: "18", value: "UTC +03:00" },
        { text: "UTC +03:30", id: "19", value: "UTC +03:30" },
        { text: "UTC +04:00", id: "20", value: "UTC +04:00" },
        { text: "UTC +04:30", id: "21", value: "UTC +04:30" },
        { text: "UTC +05:00", id: "22", value: "UTC +05:00" },
        { text: "UTC +05:30", id: "23", value: "UTC +05:30" },
        { text: "UTC +05:45", id: "24", value: "UTC +05:45" },
        { text: "UTC +06:00", id: "25", value: "UTC +06:00" },
        { text: "UTC +06:30", id: "26", value: "UTC +06:30" },
        { text: "UTC +07:00", id: "27", value: "UTC +07:00" },
        { text: "UTC +08:00", id: "28", value: "UTC +08:00" },
        { text: "UTC +09:00", id: "29", value: "UTC +09:00" },
        { text: "UTC +09:30", id: "30", value: "UTC +09:30" },
        { text: "UTC +10:00", id: "31", value: "UTC +10:00" },
        { text: "UTC +11:00", id: "32", value: "UTC +11:00" },
        { text: "UTC +12:00", id: "33", value: "UTC +12:00" },
        { text: "UTC +13:00", id: "34", value: "UTC +13:00" }
    ]
  {% endhighlight %}

#### Example - To set the dataSource with array of JSON object collection.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [timeZoneCollection]="TimeZoneData" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public TimeZoneData: any;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.TimeZoneData = {
            dataSource: [
                { text: "UTC -12:00", id: "1", value: "UTC -12:00" },
                { text: "UTC -11:00", id: "2", value: "UTC -11:00" },
                { text: "UTC -10:00", id: "3", value: "UTC -10:00" },
                { text: "UTC -09:00", id: "4", value: "UTC -09:00" },
                { text: "UTC -08:00", id: "5", value: "UTC -08:00" },
                { text: "UTC -07:00", id: "6", value: "UTC -07:00" }
            ]
        };
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00)
            }]
        };
    }

}

{% endhighlight %}

> The following are the timeZoneCollection fields that maps the appropriate column names from the dataSource.

### timeZoneCollection.text `string`
{:#members:timezonecollection-text}

Binds text field name in the dataSource to timeZoneCollection **text**. These text gets listed out in the timezone fields of the appointment window.

#### Default Value

* "text"

### timeZoneCollection.id `string`
{:#members:timezonecollection-id }

Binds id field name in the dataSource to timeZoneCollection **id**.

#### Default Value

* "id"

### timeZoneCollection.value `string`
{:#members:timezonecollection-value }

Binds value field name in the dataSource to timeZoneCollection **value**.

#### Default Value

* "value"

#### Example - To define the timeZoneCollection options by using all the above specified fields.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [timeZoneCollection]="TimeZoneData" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public TimeZoneData: any;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.TimeZoneData = {
            dataSource: [
                { text: "UTC -12:00", id: "1", value: "UTC -12:00" },
                { text: "UTC -11:00", id: "2", value: "UTC -11:00" },
                { text: "UTC -10:00", id: "3", value: "UTC -10:00" },
                { text: "UTC -09:00", id: "4", value: "UTC -09:00" },
                { text: "UTC -08:00", id: "5", value: "UTC -08:00" },
                { text: "UTC -07:00", id: "6", value: "UTC -07:00" }
            ],
            text: "text", id: "id", value: "value"
        };
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00)
            }]
        };
    }

}

{% endhighlight %}

### views `Array`
{:#members:views }

Defines the view collection to be displayed on the Schedule. By default, it displays all the views namely, Day, Week, WorkWeek and Month.

#### Default Value

* ["Day", "Week", "WorkWeek", "Month", "Agenda"]

#### Example - To display only the day and week view on the Scheduler.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [views]="ViewData" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public ViewData: any;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.ViewData = ["Day", "Week"];
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00)
            }]
        };
    }

}

{% endhighlight %}

### width `string`
{:#members:width}

Sets the width of the Schedule. Accepts both pixel and percentage values.

#### Default Value

* "100%"

#### Example - To set the width of the Schedule in pixels.

{% highlight html %}

<ej-schedule id="Schedule" width="600px" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00)
            }]
        };
    }

}

{% endhighlight %}

### enableRecurrenceValidation `boolean`
{:#members:enablerecurrencevalidation}

When set to true, Schedule allows the validation of recurrence pattern to take place before it is being assigned to the appointments. For example, when one of the instance of recurrence appointment is dragged beyond the next or previous instance of the same recurrence appointment, a pop-up is displayed with the validation message disallowing the drag functionality.

#### Default Value

* true

#### Example - To disable the RecurrenceValidation for Schedule appointments.

{% highlight html %}

<ej-schedule id="Schedule" width="600px" [currentDate]="CurrentDate" [enableRecurrenceValidation]="EnableRecurrenceValidation" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public EnableRecurrenceValidation: any;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.EnableRecurrenceValidation = false;
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00),
                Recurrence: true,
                RecurrenceRule: "FREQ=DAILY;INTERVAL=1;COUNT=10"
            }]
        };
    }

}

{% endhighlight %}

### agendaViewSettings `Object`
{:#members:agendaviewsettings}

Sets the week to display more than one week appointment summary.

### agendaViewSettings.daysInAgenda `number`
{:#members:agendaviewsettings-daysinagenda }

You can display the summary of multiple week's appointment by setting this value.

#### Default Value

* 7

#### Example - To set the daysInAgenda of agendaViewSettings.

{% highlight html %}

<ej-schedule id="Schedule" width="600px" [currentDate]="CurrentDate" [agendaViewSettings.daysInAgenda]="AgendaDaysCount" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AgendaDaysCount: number;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AgendaDaysCount = 10;
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00)
            }]
        };
    }

}

{% endhighlight %}

### agendaViewSettings.dateColumnTemplateId `string`
{:#members:agendaviewsettings-datecolumntemplateid}

You can customize the Date column display based on the requirement.

#### Default Value

* null

#### Example - To display the StartTime value in the date column of agenda View.

{% highlight html %}

<ej-schedule id="Schedule" width="600px" [currentDate]="CurrentDate" [agendaViewSettings]="AgendaViewSettings" [appointmentSettings]="AppointmentSettings"></ej-schedule>

<script id="dateColumnTemplate" type="text/x-jsrender">
    <div style="height:100%">
        <div>
            <div>{{:StartTime}}</div>
        </div>
    </div>
</script>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AgendaDaysCount: any;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AgendaDaysCount = {
            daysInAgenda: 7,
            dateColumnTemplateId: "#dateColumnTemplate"
        };
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00)
            }]
        };
    }

}

{% endhighlight %}

### agendaViewSettings.timeColumnTemplateId `string`
{:#members:agendaviewsettings-timecolumntemplateid}

You can customize the time column display based on the requirement.

#### Default Value

* null

#### Example - To display the StartTime value in the time column of agenda View.

{% highlight html %}

<ej-schedule id="Schedule" width="600px" [currentDate]="CurrentDate" [agendaViewSettings]="AgendaViewSettings" [appointmentSettings]="AppointmentSettings"></ej-schedule>

<script id="timeColumnTemplate" type="text/x-jsrender">
    <div style="height:100%">
        <div>
            <div>{{:StartTime}}</div>
        </div>
    </div>
</script>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AgendaViewSettings: any;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AgendaViewSettings = {
            daysInAgenda: 7,
            timeColumnTemplateId: "#timeColumnTemplate"
        };
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00)
            }]
        };
    }

}

{% endhighlight %}

### firstDayOfWeek `string`
{:#members:firstdayofweek}

Sets specific day as the starting day of the week.

#### Default Value

* null

#### Example - To set Saturday as starting day of the week.

{% highlight html %}

<ej-schedule id="Schedule" width="600px" [currentDate]="CurrentDate" firstDayOfWeek="Saturday" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00)
            }]
        };
    }

}

{% endhighlight %}

### workWeek `Array`
{:#members:workweek}

Sets different day collection within workWeek view.

#### Default Value

* ["Monday", "Tuesday", "Wednesday", "Thursday", "Friday"]

#### Example - To set Tuesday to Saturday as workWeek days.

{% highlight html %}

<ej-schedule id="Schedule" width="600px" [currentDate]="CurrentDate" [workWeek]="WorkWeek" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public WorkWeek: any;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.WorkWeek = ["Tuesday", "Wednesday", "Thursday", "Friday","Saturday"];
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00)
            }]
        };
    }

}

{% endhighlight %}

### tooltipSettings `Object`
{:#members:tooltipsettings}

Allows to pop-up appointment details in a tooltip while hovering over the appointments.

### tooltipSettings.enable `boolean`
{:#members:tooltipsettings-enable}

Enables or disables the tooltip display.

#### Default Value

* false

#### Example - To enable the tooltip display.

{% highlight html %}

<ej-schedule id="Schedule" width="600px" [currentDate]="CurrentDate" [tooltipSettings]="TooltipData" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public TooltipData: any;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.TooltipData = {
            enable: true
        };
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00)
            }]
        };
    }

}

{% endhighlight %}

### tooltipSettings.templateId `string`
{:#members:tooltipsettings-templateId}

Template design that customizes the tooltip. All the field names that are mapped from dataSource to the appropriate field properties within the appointmentSettings can be accessed within the template.

#### Default Value

* null

#### Example - To display the customized tooltip.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [tooltipSettings]="TooltipData" [appointmentSettings]="AppointmentSettings"></ej-schedule>

<script id="tooltip" type="text/x-jsrender">
    <div>
        <div>Subject: {{:Subject}}</div>
        <div>StartTime: {{:StartTime}}</div>
        <div>EndTime: {{:EndTime}}</div>
    </div>
</script>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public TooltipData: any;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.TooltipData = {
            enable: true,
            templateId:"#tooltip"
        };
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00)
            }]
        };
    }

}

{% endhighlight %}

### timeScale `Object`
{:#members:timescale}

Holds all the options related to the time scale of Scheduler. The timeslots either major or minor slots can be customized with this property.

### timeScale.enable `boolean`
{:#members:timescale-enable}

When set to true, displays the time slots on the Scheduler.

#### Default Value

* true

#### Example – To display the timescale on Scheduler.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [timeScale]="TimeScaleData" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public TimeScaleData: any;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.TimeScaleData = {
            enable: true
        };
        this.AppointmentSettings = {
            dataSource: [{
                EventId: 100,
                EventSubject: "Research on Sky Miracles",
                EventStartTime: new Date(2014, 4, 2, 9, 00),
                EventEndTime: new Date(2014, 4, 2, 10, 30)
            }],
            id: "EventId",
            startTime: "EventStartTime",
            endTime: "EventEndTime",
            subject: "EventSubject"
        };
    }

}

{% endhighlight %}

### timeScale.minorSlotCount `number`

{:#members:timescale-minorslotcount }

When set with some specific value, defines the number of time divisions split per hour(as per value given for the majorTimeSlot). Those time divisions are meant to be the minor slots.

#### Default Value

* 2

### timeScale.majorSlot `number`

{:#members:timescale-majorslot }

Accepts the value in minutes. When provided with specific value, displays the appropriate time interval on the Scheduler

#### Default Value

* 60

#### Example – To set the specific major and minor slots for Scheduler. 

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [timeScale]="TimeScaleData" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public TimeScaleData: any;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.TimeScaleData = {
            enable: true,
            minorSlotCount: 2,
            majorSlot: 60
        };
        this.AppointmentSettings = {
            dataSource: [{
                EventId: 100,
                EventSubject: "Research on Sky Miracles",
                EventStartTime: new Date(2014, 4, 2, 9, 00),
                EventEndTime: new Date(2014, 4, 2, 10, 30)
            }],
            id: "EventId",
            startTime: "EventStartTime",
            endTime: "EventEndTime",
            subject: "EventSubject"
        };
    }

}

{% endhighlight %}

N> When `majorTimeSlot` is provided with the value **60** and `minorTimeSlotCount` is given as **2**, then the Scheduler splits each hour into 2 timeslots with half an hour time difference for each row, which means that 30 minutes time interval is actually set to the Scheduler.

### timeScale.minorSlotTemplateId `string`
{:#members:timescale-minorslottemplateid }

Template design that customizes the timecells (minor slots) that are partitioned based on minorSlotCount. Accepts id value of the template defined for minor time slots.

#### Default Value

* null

### timeScale.majorSlotTemplateId `string`
{:#members:timescale-majorslottemplateid }

Template design that customizes the timecells (major slots). Accepts id value of the template defined for major time slots.

#### Default Value

* null

#### Example – To set the template for minor slots and major slots.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [timeScale]="TimeScaleData" [appointmentSettings]="AppointmentSettings"></ej-schedule>

<script id="timeMinorTemplate" type="text/x-jsrender">
    <div style='font-size:9px !important;'>{{:~timeMinorTemp(date)}}</div>
</script>

<script id="timeMajorTemplate" type="text/x-jsrender">
    <div style='font-size:9px !important;'>{{:~timeMajorTemp(date)}}</div>
</script>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public TimeScaleData: any;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.TimeScaleData = {
            enable: true,
            minorSlotCount: 2,
            majorSlot: 60,
            majorSlotTemplate:"#timeMinorTemplate",
            minorSlotTemplate:"#timeMajorTemplate"
        };
        this.AppointmentSettings = {
            dataSource: [{
                EventId: 100,
                EventSubject: "Research on Sky Miracles",
                EventStartTime: new Date(2014, 4, 2, 9, 00),
                EventEndTime: new Date(2014, 4, 2, 10, 30)
            }],
            id: "EventId",
            startTime: "EventStartTime",
            endTime: "EventEndTime",
            subject: "EventSubject"
        };
        $.views.helpers({ timeMinorTemp: _timeMinorFormat, timeMajorTemp: _timeMajorFormat });
    }

    _timeMinorFormat(date) {
        var tFormat = Globalize.format(new Date(date),"hh:mm:ss tt");
        return tFormat;
    }

    _timeMajorFormat(date) {
        var tFormat = Globalize.format(new Date(date), "mm:ss ");
        return tFormat;
    }
}

{% endhighlight %}

### showDeleteConfirmationDialog `boolean`
{:#members:showdeleteconfirmationdialog}

When set to true, shows the delete confirmation dialog before deleting an appointment.

#### Default Value

* true

#### Example – To hide the display of delete confirmation dialog.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [showDeleteConfirmationDialog]="DeleteConfirmationDialog" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public DeleteConfirmationDialog: boolean;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.DeleteConfirmationDialog = false;
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00)
            }]
        };
    }

}

{% endhighlight %}

### allDayCellsTemplateId  `string`
{:#members:alldaycellstemplateid}

Accepts the id value of the template layout defined for the all-day cells and customizes it.

#### Default Value

* null

#### Example - To display the customized all-day cells.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" allDayCellsTemplateId="#dateColumnTemplate" [appointmentSettings]="AppointmentSettings"></ej-schedule>

<script id="dateColumnTemplate" type="text/x-jsrender">
    <div style="height:100%">
        <div></div>
    </div>
</script>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00)
            }]
        };
    }

}

{% endhighlight %}

### workCellsTemplateId  `string`
{:#members:workcellstemplateid}

Accepts the id value of the template layout defined for the work cells and month cells.

#### Default Value

* null

#### Example - To display the customized Scheduler cells.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" workCellsTemplateId="#workTemplate" [appointmentSettings]="AppointmentSettings"></ej-schedule>

<script id="workTemplate" type="text/x-jsrender">
    <div style="height:100%">
        <div></div>
    </div>
</script>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00)
            }]
        };
    }

}

{% endhighlight %}

### dateHeaderTemplateId  `string`
{:#members:dateheadertemplateid}

Accepts the id value of the template layout defined for the date header cells and customizes it.

#### Default Value

* null

#### Example - To display the customized header cells.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" dateHeaderTemplateId="#workTemplate" [appointmentSettings]="AppointmentSettings"></ej-schedule>

<script id="dateColumnTemplate" type="text/x-jsrender">
    <div style="height:100%">
        <div></div>
    </div>
</script>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00)
            }]
        };
    }

}

{% endhighlight %}

### showOverflowButton `boolean`
{:#members:showoverflowbutton}

when set to false, allows the height of the work-cells to adjust automatically (either expand or collapse) based on the number of appointment count it has.

#### Default Value

* true

#### Example – To auto adjust cell height, set showOverflowButton to false.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [showOverflowButton]="ShowOverflowButton" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public ShowOverflowButton: boolean;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.ShowOverflowButton = false;
        this.AppointmentSettings = {
            dataSource: [{
                EventId: 100,
                EventSubject: "Research on Sky Miracles",
                EventStartTime: new Date(2014, 4, 2, 9, 00),
                EventEndTime: new Date(2014, 4, 2, 10, 30)
            }],
            id: "EventId",
            startTime: "EventStartTime",
            endTime: "EventEndTime",
            subject: "EventSubject"
        };
    }

}

{% endhighlight %}

### appointmentDragArea `string`
{:#members:appointmentdragarea}

Allows setting draggable area for the Scheduler appointments. Also, turns on the external drag and drop, when set with some specific external drag area name.

#### Default Value

* ""

#### Example - To enable external drag and drop support.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" appointmentDragArea="body" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00)
            }]
        };
    }

}

{% endhighlight %}

### showNextPrevMonth `boolean`
{:#members:shownextprevmonth}

When set to true, displays the other months days from the current month on the Schedule.

#### Default Value

* true

#### Example - To hide the other months days from the current month.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" currentView="month" [showNextPrevMonth]="ShowNextPrevMonth" [appointmentSettings]="AppointmentSettings"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public ShowNextPrevMonth: boolean;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.ShowNextPrevMonth = false;
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00)
            }]
        };
    }

}

{% endhighlight %}

### blockoutSettings `Object`
{:#members:blockoutsettings}

Blocks the user-specific time interval on the Scheduler, so that no appointments can be created on that particular time slots. It includes the dataSource option and also the fields related to block intervals.

### blockoutSettings.enable `boolean`
{:#members:blockoutsettings-enable}

When set to true, enables the blockout option to be applied on the Scheduler cells.

#### Default Value

* false

#### Example - To enable the block intervals option.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" currentView="month" [blockoutSettings]="BlockoutData"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public BlockoutData: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.BlockoutData = {
            enable: true,
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 12, 00)
            }]
        };
    }

}

{% endhighlight %}

### blockoutSettings.templateId `string`
{:#members:blockoutsettings-templateid}

Template design that applies on the Schedule block intervals. All the field names that are mapped from dataSource to the appropriate field properties within the blockoutSettings can be used within the template.

#### Default Value

* null

#### Example - To set the block intervals template.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" currentView="month" [blockoutSettings]="BlockoutData"></ej-schedule>

<script id="blockTemplate" type="text/x-jsrender">
   <div style="height:100%">
      <div>{{:Subject}}</div>
   </div>
</script>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public BlockoutData: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.BlockoutData = {
            enable: true,
            templateId: "#blockTemplate",
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 11, 00)
            }]
        };
    }

}

{% endhighlight %}

### blockoutSettings.dataSource `Object|Array`
{:#members:blockoutsettings-datasource}

The dataSource option accepts either JSON object collection or DataManager ([ej.DataManager](/js/datamanager/overview)) instance that contains Schedule block intervals.

#### Default Value

* []

#### Example - To set the dataSource with array of JSON object collection.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" currentView="month" [blockoutSettings]="BlockoutData"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public BlockoutData: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.BlockoutData = {
            enable:true,
            dataSource: [{
                Id: 101,
                Subject: "Service",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 12, 00)
            }, {
                Id: 102,
                Subject: "Bad Monsoon",
                StartTime: new Date(2014, 4, 5, 05, 00),
                EndTime: new Date(2014, 4, 5, 07, 00)
            }]
        };
    }

}

{% endhighlight %}

#### Example - To set the dataSource with data manager instance.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" currentView="month" [blockoutSettings]="BlockoutData"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public BlockoutData: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.BlockoutData = {
            enable:true,
            dataSource: ej.DataManager({
                url: "http://mvc.syncfusion.com/OdataServices/Northwnd.svc/Events",
                crossDomain: true
            })
        };
    }

}

{% endhighlight %}

### blockoutSettings.query `string`
{:#members:blockoutsettings-query}

It holds either the ej.Query() object or simply the query string that retrieves the specified records from the table.

#### Default Value

* null

#### Example - Query the data manager to fetch specific record count from the Events table.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" currentView="month" [blockoutSettings]="BlockoutData"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public BlockoutData: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.BlockoutData = {
            enable:true,
            dataSource: ej.DataManager({
                url: "http://mvc.syncfusion.com/OdataServices/Northwnd.svc/Events",
                crossDomain: true
            }),
            query: ej.Query().from("Events").take(10)
        };
    }

}

{% endhighlight %}

### blockoutSettings.tableName `string`
{:#members:blockoutsettings-tablename}

Assign the table name from where the records are to be fetched for the Schedule.

#### Default Value

* null

#### Example - Using tableName property to fetch all the records directly from it.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" currentView="month" [blockoutSettings]="BlockoutData"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public BlockoutData: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.BlockoutData = {
            enable:true,
            dataSource: ej.DataManager({
                url: "http://mvc.syncfusion.com/OdataServices/Northwnd.svc/Events",
                crossDomain: true
            }),
            tableName: "Events"
        };
    }

}

{% endhighlight %}

> The following are the block time fields that holds the appropriate column names from the dataSource. All its default values are `null`.

### blockoutSettings.id `string`
{:#members:blockoutsettings-id}

Binds the id field name in dataSource to the id of block time interval. It denotes the unique id assigned to each of the block records.

#### Default Value

* null

### blockoutSettings.startTime `string`
{:#members:blockoutsettings-starttime}

Binds the name of startTime field in the dataSource with start time of block time interval. It indicates the date and time, when the block interval actually starts in the Scheduler.

#### Default Value

* null

### blockoutSettings.endTime `string`
{:#members:blockoutsettings-endtime}

Binds the name of endTime field in dataSource with the end time of block time interval. It indicates the date and time, when the block interval actually ends in the Scheduler.

#### Default Value

* null

#### Example - To create a block intervals with the fields id, startTime and endTime.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" currentView="month" [blockoutSettings]="BlockoutData"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public BlockoutData: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.BlockoutData = {
            enable: true,
            dataSource: [{
                BlockId: 101,
                BlockStartTime: new Date(2014, 4, 5, 10, 00),
                BlockEndTime: new Date(2014, 4, 5, 11, 00)
            }],
            id: "BlockId",
            startTime: "BlockStartTime",
            endTime: "BlockEndTime"
        };
    }

}

{% endhighlight %}

> The fields startTime and endTime are mandatory fields to create the block intervals.

### blockoutSettings.subject `string`
{:#members:blockoutsettings-subject}

Binds the name of subject field in the dataSource to block time Subject. Indicates the Subject or title that gets displayed on the Schedule block intervals.

#### Default Value

* null

#### Example - The block intervals with Subject.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" currentView="month" [blockoutSettings]="BlockoutData"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public BlockoutData: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.BlockoutData = {
            enable: true,
            dataSource: [{
                BlockId: 101,
                BlockStartTime: new Date(2014, 4, 5, 10, 00),
                BlockEndTime: new Date(2014, 4, 5, 11, 00),
                BlockSubject: "Holiday"
            }],
            id: "BlockId",
            startTime: "BlockStartTime",
            endTime: "BlockEndTime",
            subject: "BlockSubject"
        };
    }

}

{% endhighlight %}

### blockoutSettings.isBlockAppointment `string`
{:#members:blockoutsettings-isblockappointment}

Binds the name of `isBlockAppointment` field in dataSource. When set to true, disables the appointments that lies on the blocked area and restrict to perform CRUD operations in it.

#### Default Value

* null

#### Example - To restrict the CRUD operations on the appointments that lies behind the blocked intervals.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" currentView="month" [blockoutSettings]="BlockoutData"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public BlockoutData: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.BlockoutData = {
            enable: true,
            dataSource: [{
                BlockId: 101,
                BlockStartTime: new Date(2014, 4, 5, 10, 00),
                BlockEndTime: new Date(2014, 4, 5, 11, 00),
                BlockSubject: "Holiday",
                IsBlockAppointment: true
            }],
            id: "BlockId",
            startTime: "BlockStartTime",
            endTime: "BlockEndTime",
            subject: "BlockSubject",
            isBlockAppointment: "IsBlockAppointment"
        };
    }

}

{% endhighlight %}

### blockoutSettings.isAllDay `string`
{:#members:blockoutsettings-isallday}

Binds the name of `isAllDay` field in dataSource. It indicates whether an entire day is blocked or not.

#### Default Value

* null

#### Example - To limits the entire day

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" currentView="month" [blockoutSettings]="BlockoutData"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public BlockoutData: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.BlockoutData = {
            enable: true,
            dataSource: [{
                BlockId: 101,
                BlockStartTime: new Date(2014, 4, 5, 10, 00),
                BlockEndTime: new Date(2014, 4, 5, 11, 00),
                BlockSubject: "Holiday",
                IsBlockAppointment: true,
                FullDay: true
            }],
            id: "BlockId",
            startTime: "BlockStartTime",
            endTime: "BlockEndTime",
            subject: "BlockSubject",
            isBlockAppointment: "IsBlockAppointment",
            isAllDay: "FullDay"
        };
    }

}

{% endhighlight %}

### blockoutSettings.resourceId `string`
{:#members:blockoutsettings-resourceid}

Binds the name of `resourceId` field in dataSource. Specifies the id of the resources, to which the time intervals are needed to be blocked.

#### Default Value

* null

#### Example - Block intervals for multiple resources scenario.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" currentView="month" [group]="GroupData" [resources]="ResourceData" [blockoutSettings]="BlockoutData"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public GroupData: any;
    public ResourceData: any;
    public BlockoutData: any;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.GroupData = {
            resources: ["Owners"]
        };
        this.ResourceData = [{
            field: "ownerId",
            title: "Owner",
            name: "Owners",
            allowMultiple: true,
            resourceSettings: {
                dataSource: [
                    { text: "Nancy", id: 1, color: "#f8a398" },
                    { text: "Steven", id: 2, color: "#56ca85"}
                ],
                text: "text", id: "id", color: "color"
            }
        }];
        this.BlockoutData = {
            enable: true,
            dataSource: [{
                BlockId: 101,
                BlockStartTime: new Date(2014, 4, 5, 10, 00),
                BlockEndTime: new Date(2014, 4, 5, 11, 00),
                BlockSubject: "Holiday",
                IsBlockAppointment: true,
                FullDay: true
            }],
            id: "BlockId",
            startTime: "BlockStartTime",
            endTime: "BlockEndTime",
            subject: "BlockSubject",
            isBlockAppointment: "IsBlockAppointment",
            isAllDay: "FullDay"
        };
        this.AppointmentSettings = {
            dataSource: [{
                EventId: 100,
                EventSubject: "Research on Sky Miracles",
                EventStartTime: new Date(2014, 4, 2, 9, 00),
                EventEndTime: new Date(2014, 4, 2, 10, 30),
                ownerId: 2
            }],
            id: "EventId",
            startTime: "EventStartTime",
            endTime: "EventEndTime",
            subject: "EventSubject",
            resourceFields: "ownerId"
        };
    }

}

{% endhighlight %}

### blockoutSettings.groupId `string`
{:#members:blockoutsettings-resourceid}

Binds the name of `groupId` field in dataSource. Specifies the id of the resource group, to which the time intervals are needed to be blocked.

#### Default Value

* null

#### Example - Block intervals for multiple resources scenario.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" currentView="month" [group]="GroupData" [resources]="ResourceData" [blockoutSettings]="BlockoutData"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public GroupData: any;
    public ResourceData: any;
    public BlockoutData: any;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.GroupData = {
            resources: ["Owners", "Rooms"]
        };
        this.ResourceData = [{
            field: "ownerId",
            title: "Owner",
            name: "Owners",
            resourceSettings: {
                dataSource: [
                    { OwnerText: "Nancy", id: 1, OwnerColor: "#f8a398" },
                    { OwnerText: "Steven", id: 2, OwnerColor: "#56ca95" }
                ],
                text: "OwnerText", id: "id", color: "OwnerColor"
            }
        }, {
            field: "roomId",
            title: "Room(s)",
            name: "Rooms",
            resourceSettings: {
                dataSource: [
                    { text: "Room1", id: 1, groupId: 1, color: "#f8a398" },
                    { text: "Room2", id: 2, groupId: 2, color: "#56ca85" },
                    { text: "Room3", id: 3, groupId: 2, color: "#56ac88" }
                ],
                text: "text", id: "id", color: "color", groupId: "groupId"
            }
        }];
        this.BlockoutData = {
            enable: true,
            dataSource: [{
                BlockId: 101,
                BlockStartTime: new Date(2014, 4, 1, 10, 00),
                BlockEndTime: new Date(2014, 4, 1, 11, 00),
                BlockSubject: "Travel",
                IsBlockAppointment: true,
                BlockResId: 2,
                BlockGrpId: 1,
            }],
            id: "BlockId",
            startTime: "BlockStartTime",
            endTime: "BlockEndTime",
            subject: "BlockSubject",
            isBlockAppointment: "IsBlockAppointment",
            resourceId: "BlockResId",
            groupId: "BlockGrpId",
        };
        this.AppointmentSettings = {
            dataSource: [{
                EventId: 100,
                EventSubject: "Research on Sky Miracles",
                EventStartTime: new Date(2014, 4, 2, 9, 00),
                EventEndTime: new Date(2014, 4, 2, 10, 30),
                ownerId: 2,
                roomId: 1
            }],
            id: "EventId",
            startTime: "EventStartTime",
            endTime: "EventEndTime",
            subject: "EventSubject",
            resourceFields: "ownerId,roomId"
        };
    }

}

{% endhighlight %}

### blockoutSettings.customStyle `string`
{:#members:blockoutsettings-customstyle}

Binds the name of `customStyle` field in dataSource. It applies the custom CSS to the block intervals.

#### Default Value

* null

#### Example - The block intervals with custom style.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [blockoutSettings]="BlockoutData"></ej-schedule>

<style type="text/css">
    .custom-css {
        background-color: Teal !important;
    }
</style>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public BlockoutData: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.BlockoutData = {
            enable: true,
            dataSource: [{
                BlockId: 101,
                BlockStartTime: new Date(2014, 4, 5, 10, 00),
                BlockEndTime: new Date(2014, 4, 5, 11, 00),
                BlockSubject: "Service",
                IsBlockAppointment: true,
                BlockStyle: "custom-css"
            }],
            id: "BlockId",
            startTime: "BlockStartTime",
            endTime: "BlockEndTime",
            subject: "BlockSubject",
            isBlockAppointment: "IsBlockAppointment",
            customStyle: "BlockStyle"
        };
    }

}

{% endhighlight %}

## Methods

### deleteAppointment(data)
{:#methods:deleteappointment}

This method is used to delete the appointment based on the guid value or the appointment data passed to it.

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
            <td class="name">data</td>
            <td class="type">string|Object</td>
            <td class="description">GUID value of an appointment element or an appointment object</td>
        </tr>
    </tbody>
</table>

#### Returns:
{:#methods:returns:}

void

#### Example - Using GUID Value

The following code snippet explain how to delete an appointment by using the GUID, while clicking an appointment.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings" (appointmentClick)="onAppointmentClick($event)"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 1,
                Subject: "Music Class",
                StartTime: new Date("2015/11/7 06:00 AM"),
                EndTime: new Date("2015/11/7 07:00 AM")
            }, {
                Id: 2,
                Subject: "School",
                StartTime: new Date("2015/11/7 9:00 AM"),
                EndTime: new Date("2015/11/7 02:30 PM")
            }]
        };
    }

    onAppointmentClick(args) {
        var schObj = $("#schedule").data("ejSchedule");
        schObj.deleteAppointment(args.appointment.Guid);
        // $(".e-appointment").eq(0).attr("guid") --> To get the guid attribute value of an element directly.
    }

}

{% endhighlight %}

#### Example - Using Appointment Object

The following code snippet explain how to delete an appointment by passing appointment object, while clicking an appointment.

{% highlight html %}

<ej-schedule id="Schedule" width="100%" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings" (appointmentClick)="onAppointmentClick($event)"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 1,
                Subject: "Music Class",
                StartTime: new Date("2015/11/7 06:00 AM"),
                EndTime: new Date("2015/11/7 07:00 AM")
            }, {
                Id: 2,
                Subject: "School",
                StartTime: new Date("2015/11/7 9:00 AM"),
                EndTime: new Date("2015/11/7 02:30 PM")
            }]
        };
    }

    onAppointmentClick(args) {
        var schObj = $("#schedule").data("ejSchedule");
        schObj.deleteAppointment(args.appointment);
    }

}

{% endhighlight %}

### destroy()
{:#methods:destroy}

Destroys the Schedule widget. All the events bound using this._on are unbound automatically and the control is moved to pre-init state.

#### Returns:
{:#methods:returns:}

void

#### Example

{% highlight html %}

<ej-schedule id="Schedule"></ej-schedule>

<script type="text/javascript">

$('#Schedule').ejSchedule();
var schObj = $("#Schedule").data("ejSchedule");
schObj.destroy(); // destroy the schedule

</script>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    constructor() { }

}

{% endhighlight %}

### exportSchedule(action, serverEvent, id)
{:#methods:exportschedule}

Exports the appointments from the Schedule control.

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
            <td class="name">action</td>
            <td class="type">string</td>
            <td class="description">It refers the controller action name to redirect. (For MVC)</td>
        </tr>
        <tr>
            <td class="name">serverEvent</td>
            <td class="type">string</td>
            <td class="description">It refers the server event name.(For ASP)</td>
        </tr>
        <tr>
            <td class="name">id</td>
            <td class="type">string|number</td>
            <td class="description">Pass the id of an appointment, in case if a single appointment needs to be exported. Otherwise, it takes the null value.</td>
        </tr>
    </tbody>
</table>

#### Returns:
{:#methods:returns:}

void

#### Example

{% highlight html %}

<ej-schedule id="Schedule" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings"></ej-schedule>

<script type="text/javascript">

var schObj = $("#Schedule").data("ejSchedule");
schObj.exportSchedule("ActionName","ExportToICS", null); // To Export all the Appointments
schObj.exportSchedule("ActionName","ExportToICS", 101); // To Export a single appointment with an id "101"

</script>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 12, 00),
                StartTimeZone: "UTC +00:00",
                EndTimeZone: "UTC +00:00"
            }, {
                Id: 102,
                Subject: "Play with pets",
                StartTime: new Date(2014, 4, 5, 05, 00),
                EndTime: new Date(2014, 4, 5, 07, 00),
                StartTimeZone: "UTC +00:00",
                EndTimeZone: "UTC +00:00"
            }],
            id: "Id",
            startTime: "StartTime",
            endTime: "EndTime",
            subject: "Subject",
            startTimeZone: "StartTimeZone",
            endTimeZone: "EndTimeZone"
       };
    }

}

{% endhighlight %}

### saveAsExcel(action, serverEvent, type)
{:#methods:saveasexcel}

Exports the appointments from the Schedule control.

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
            <td class="name">action</td>
            <td class="type">string</td>
            <td class="description">It refers the controller action name to redirect. (For MVC)</td>
        </tr>
        <tr>
            <td class="name">serverEvent</td>
            <td class="type">string</td>
            <td class="description">It refers the server event name.(For ASP)</td>
        </tr>
        <tr>
            <td class="name">type</td>
            <td class="type">boolean</td>
            <td class="description">To export all appointments including individual occurrences or excluding the individual occurrences of recurrence appointments. </td>
        </tr>
    </tbody>
</table>

#### Returns:
{:#methods:returns:}

void

#### Example

{% highlight html %}

<ej-schedule id="Schedule" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings"></ej-schedule>

<script type="text/javascript">

var schObj = $("#Schedule").data("ejSchedule");
schObj.saveAsExcel("ActionName", null, true); // To Export all the Appointments including ocurrences
schObj.saveAsExcel("ActionName", null, false); // To Export all the Appointments excluding ocurrences

</script>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 12, 00),
                StartTimeZone: "UTC +00:00",
                EndTimeZone: "UTC +00:00"
            }, {
                Id: 102,
                Subject: "Play with pets",
                StartTime: new Date(2014, 4, 5, 05, 00),
                EndTime: new Date(2014, 4, 5, 07, 00),
                StartTimeZone: "UTC +00:00",
                EndTimeZone: "UTC +00:00"
            }],
            id: "Id",
            startTime: "StartTime",
            endTime: "EndTime",
            subject: "Subject",
            startTimeZone: "StartTimeZone",
            endTimeZone: "EndTimeZone"
       };
    }

}

{% endhighlight %}

### filterAppointments(filterConditions)
{:#methods:filterappointments}

Searches and filters the appointments from appointment list of Schedule control.

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
            <td class="name">filterConditions</td>
            <td class="type">Array</td>
            <td class="description">Holds array of one or more conditional objects for filtering the appointments based on it.</td>
        </tr>
    </tbody>
</table>

#### Returns:
{:#methods:returns:}

Array

#### Example

{% highlight html %}

<ej-schedule id="Schedule" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings"></ej-schedule>

<script type="text/javascript">

var schObj = $("#Schedule").data("ejSchedule");
var filter=[{
   field: "Subject",
   operator: "contains",
   value: "with",
   predicate: "or"
}];
var appointments = schObj.filterAppointments(filter); // filters the appointments list of Schedule control

</script>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 12, 00),
                StartTimeZone: "UTC +00:00",
                EndTimeZone: "UTC +00:00
            }, {
                Id: 102,
                Subject: "Play with pets",
                StartTime: new Date(2014, 4, 5, 05, 00),
                EndTime: new Date(2014, 4, 5, 07, 00),
                StartTimeZone: "UTC +00:00",
                EndTimeZone: "UTC +00:00
            }, {
                Id: 103,
                Subject: "Reading books",
                StartTime: new Date(2014, 4, 5, 08, 00),
                EndTime: new Date(2014, 4, 5, 09, 00),
                StartTimeZone: "UTC +00:00",
                EndTimeZone: "UTC +00:00
            }],
            id: "Id",
            startTime: "StartTime",
            endTime: "EndTime",
            subject: "Subject",
            startTimeZone: "StartTimeZone",
            endTimeZone: "EndTimeZone"
       };
    }

}

{% endhighlight %}

### getAppointments()
{:#methods:getappointments}

Gets the complete appointment list of Schedule control.

#### Returns:
{:#methods:returns:}

Array

#### Example

{% highlight html %}

<ej-schedule id="Schedule" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings"></ej-schedule>

<script type="text/javascript">

var schObj = $("#Schedule").data("ejSchedule");
var appointments=schObj.getAppointments(); // Gets the appointments list of Schedule control

</script>

{% endhighlight %}

### print(data)
{:#methods:print}

Prints the entire Scheduler or a single appointment based on the appointment data passed as an argument to it. Simply calling the print() method, without passing any argument will print the entire Scheduler.

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
            <td class="name">data</td>
            <td class="type">Object</td>
            <td class="description">Either accepts no arguments at all or else accepts an appointment object.</td>
        </tr>
    </tbody>
</table>

#### Returns:
{:#methods:returns:}

void

#### Example

{% highlight html %}

<ej-schedule id="Schedule" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings" (appointmentClick)="onAppointmentClick($event)"></ej-schedule>

<script type="text/javascript">

// Use the below 2 lines of code within any particular action like button click to print the entire Scheduler.
var schObj = $("#Schedule").data("ejSchedule");
schObj.print(); // Prints entire Scheduler with all appointments

</script>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 12, 00),
                Recurrence:false,
                RecurrenceRule:null,
                StartTimeZone: "UTC +00:00",
                EndTimeZone: "UTC +00:00
            }, {
                Id: 102,
                Subject: "Play with pets",
                StartTime: new Date(2014, 4, 5, 05, 00),
                EndTime: new Date(2014, 4, 5, 07, 00),
                Recurrence:true,
                RecurrenceRule:"FREQ=DAILY;INTERVAL=1;COUNT=10",
                StartTimeZone: "UTC +00:00",
                EndTimeZone: "UTC +00:00
            }],
            id: "Id",
            startTime: "StartTime",
            endTime: "EndTime",
            subject: "Subject",
            recurrence:"Recurrence",
            recurrenceRule:"RecurrenceRule",
            startTimeZone: "StartTimeZone",
            endTimeZone: "EndTimeZone"
       };
    }

    onAppointmentClick(args) {
        var schObj = $("#Schedule").data("ejSchedule");
        schObj.print(args.appointment); //Print specific appointment
    }

}

{% endhighlight %}

### refreshScroller()
{:#methods:refreshscroller}

Refreshes the Scroller of Scheduler while using it within some other controls or application.

#### Returns:
{:#methods:returns:}

void

#### Example

{% highlight html %}

<ej-schedule id="Schedule" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings"></ej-schedule>

<script type="text/javascript">

var schObj = $("#Schedule").data("ejSchedule");
schObj.refreshScroller(); // To refresh scroller while using Schedule control in some other control

</script>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 12, 00),
                Recurrence:false,
                RecurrenceRule:null,
                StartTimeZone: "UTC +00:00",
                EndTimeZone: "UTC +00:00
            }, {
                Id: 102,
                Subject: "Play with pets",
                StartTime: new Date(2014, 4, 5, 05, 00),
                EndTime: new Date(2014, 4, 5, 07, 00),
                Recurrence:true,
                RecurrenceRule:"FREQ=DAILY;INTERVAL=1;COUNT=10",
                StartTimeZone: "UTC +00:00",
                EndTimeZone: "UTC +00:00
            }],
            id: "Id",
            startTime: "StartTime",
            endTime: "EndTime",
            subject: "Subject",
            recurrence:"Recurrence",
            recurrenceRule:"RecurrenceRule",
            startTimeZone: "StartTimeZone",
            endTimeZone: "EndTimeZone"
       };
    }

}

{% endhighlight %}

### saveAppointment(appointmentObject)

{:#methods:saveappointment}

It is used to save the appointment. The appointment object is based on the argument passed to this method.

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
            <td class="name">appointmentObject</td>
            <td class="type">Object</td>
            <td class="description">appointment object which includes appointment details</td>
        </tr>
    </tbody>
</table>

#### Returns:
{:#methods:returns:}

Void

#### Example

{% highlight html %}

<ej-schedule id="Schedule" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings"></ej-schedule>

<script type="text/javascript">

var obj = {
    Id: 108,
    Subject: "Talk with Nature",
    StartTime: new Date(2014, 4, 5, 10, 00),
    EndTime: new Date(2014, 4, 5, 12, 00),
    AllDay: true,
    Recurrence: false,
    RecurrenceRule: null,
    StartTimeZone: "UTC +00:00",
    EndTimeZone: "UTC +00:00"
};
var schObj = $("#Schedule").data("ejSchedule");
schObj.saveAppointment(obj); //obj contains collection of appointment.

</script>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 12, 00),
                Recurrence:false,
                RecurrenceRule:null,
                StartTimeZone: "UTC +00:00",
                EndTimeZone: "UTC +00:00
            }, {
                Id: 102,
                Subject: "Play with pets",
                StartTime: new Date(2014, 4, 5, 05, 00),
                EndTime: new Date(2014, 4, 5, 07, 00),
                Recurrence:true,
                RecurrenceRule:"FREQ=DAILY;INTERVAL=1;COUNT=10",
                StartTimeZone: "UTC +00:00",
                EndTimeZone: "UTC +00:00
            }],
            id: "Id",
            startTime: "StartTime",
            endTime: "EndTime",
            subject: "Subject",
            recurrence:"Recurrence",
            recurrenceRule:"RecurrenceRule",
            startTimeZone: "StartTimeZone",
            endTimeZone: "EndTimeZone"
       };
    }

}

{% endhighlight %}

### getRecurrenceRule()
{:#methods:getrecurrencerule}

Generate the recurrence rule as a string, based on the repeat options selected.

#### Returns:
{:#methods:returns:}

string

#### Example

{% highlight html %}

<div ej-recurrenceeditor id="RecurrenceEditor"></div>

<script type="text/javascript">

var obj = $("#RecurrenceEditor").data("ejRecurrenceEditor");
alert( obj.getRecurrenceRule()); // Display the recurrence rule

</script>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    constructor() { }

}

{% endhighlight %}

### getSlotByElement(element)

{:#methods:getslotbyelement}

Retrieves the time slot information (start/end time and resource details) of the given element. The parameter is optional - as when no element is passed to it, the currently selected cell information will be retrieved. When multiple cells are selected in the Scheduler, it is not necessary to provide the parameter.

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
            <td class="name">element</td>
            <td class="type">Object</td>
            <td class="description">TD element object rendered as Scheduler work cell</td>
        </tr>
    </tbody>
</table>

#### Returns:
{:#methods:returns:}

Object

#### Example

{% highlight html %}

<ej-schedule id="Schedule" [currentDate]="CurrentDate"></ej-schedule>

<script type="text/javascript">

var obj = $("#Schedule1").data("ejSchedule");
var $td = $(".e-draggableworkarea table tr td").first();
var slotDetails = obj.getSlotByElement($td);

console.log("Start Date: " + slotDetails.startTime);
console.log("End Date: " + slotDetails.endTime);
console.log("Resource details: " + slotDetails.resources);

</script>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
    }

}

{% endhighlight %}

### searchAppointments(searchString, field, operator, ignoreCase)
{:#methods:searchappointments}

Searches the appointments from the appointment list of Schedule control based on the provided search string in its argument list.

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
            <td class="name">searchString</td>
            <td class="type">Object|string</td>
            <td class="description">Defines the search word or the filter condition, based on which the appointments are filtered from the list.</td>
        </tr>
        <tr>
            <td class="name">field</td>
            <td class="type">string</td>
            <td class="description">Defines the field name on which the search is to be made.</td>
        </tr>
        <tr>
            <td class="name">operator</td>
            <td class="type">enum|string<ts ref="ej.FilterOperators"/></td>
            <td class="description">Defines the filterOperator value for the search operation.</td>
        </tr>
        <tr>
            <td class="name">ignoreCase</td>
            <td class="type">boolean</td>
            <td class="description">Defines the ignoreCase value for performing the search operation.</td>
        </tr>
    </tbody>
</table>

#### Returns:
{:#methods:returns:}

Array

#### Example

{% highlight html %}

<ej-schedule id="Schedule" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings"></ej-schedule>

<script type="text/javascript">

var schObj = $("#Schedule").data("ejSchedule");
var appointments=schObj.searchAppointments("with"); // Searches the appointments list of Schedule control for the appointments containing the word "with"

</script>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 12, 00),
                StartTimeZone: "UTC +00:00",
                EndTimeZone: "UTC +00:00"
            }, {
                Id: 102,
                Subject: "Play with pets",
                StartTime: new Date(2014, 4, 5, 05, 00),
                EndTime: new Date(2014, 4, 5, 07, 00),
                StartTimeZone: "UTC +00:00",
                EndTimeZone: "UTC +00:00"
            }, {
                Id: 103,
                Subject: "Reading books",
                StartTime: new Date(2014, 4, 5, 08, 00),
                EndTime: new Date(2014, 4, 5, 09, 00),
                StartTimeZone: "UTC +00:00",
                EndTimeZone: "UTC +00:00"
            }],
            id: "Id",
            startTime: "StartTime",
            endTime: "EndTime",
            subject: "Subject",
            startTimeZone: "StartTimeZone",
            endTimeZone: "EndTimeZone"
        };
    }

}

{% endhighlight %}

### refresh()
{:#methods:refresh}

Refreshes the entire Schedule control.

#### Returns:
{:#methods:returns:}

void

#### Example

{% highlight html %}

<ej-schedule id="Schedule" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings"></ej-schedule>

<script type="text/javascript">

var schObj = $("#Schedule").data("ejSchedule");
schObj.refresh(); // To refresh the Schedule control within the client side event

</script>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 12, 00),
                StartTimeZone: "UTC +00:00",
                EndTimeZone: "UTC +00:00"
            }, {
                Id: 102,
                Subject: "Play with pets",
                StartTime: new Date(2014, 4, 5, 05, 00),
                EndTime: new Date(2014, 4, 5, 07, 00),
                StartTimeZone: "UTC +00:00",
                EndTimeZone: "UTC +00:00"
            }, {
                Id: 103,
                Subject: "Reading books",
                StartTime: new Date(2014, 4, 5, 08, 00),
                EndTime: new Date(2014, 4, 5, 09, 00),
                StartTimeZone: "UTC +00:00",
                EndTimeZone: "UTC +00:00"
            }],
            id: "Id",
            startTime: "StartTime",
            endTime: "EndTime",
            subject: "Subject",
            startTimeZone: "StartTimeZone",
            endTimeZone: "EndTimeZone"
        };
    }

}

{% endhighlight %}

### refreshAppointments()
{:#methods:refreshappointments}

Refreshes only the appointment elements within the Schedule control.

#### Returns:
{:#methods:returns:}

void

#### Example

{% highlight html %}

<ej-schedule id="Schedule" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings"></ej-schedule>

<script type="text/javascript">

var schObj = $("#Schedule").data("ejSchedule");
schObj.refreshAppointments(); // To refresh all the appointments within Scheduler

</script>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 12, 00),
                StartTimeZone: "UTC +00:00",
                EndTimeZone: "UTC +00:00"
            }, {
                Id: 102,
                Subject: "Play with pets",
                StartTime: new Date(2014, 4, 5, 05, 00),
                EndTime: new Date(2014, 4, 5, 07, 00),
                StartTimeZone: "UTC +00:00",
                EndTimeZone: "UTC +00:00"
            }, {
                Id: 103,
                Subject: "Reading books",
                StartTime: new Date(2014, 4, 5, 08, 00),
                EndTime: new Date(2014, 4, 5, 09, 00),
                StartTimeZone: "UTC +00:00",
                EndTimeZone: "UTC +00:00"
            }],
            id: "Id",
            startTime: "StartTime",
            endTime: "EndTime",
            subject: "Subject",
            startTimeZone: "StartTimeZone",
            endTimeZone: "EndTimeZone"
        };
    }

}

{% endhighlight %}

### notifyChanges(action, data)
{:#methods:notifychanges}

Passes the server-side action and data to the client-side for rendering the modified appointment list on the Schedule control.

#### Returns:
{:#methods:returns:}

void

#### Example

{% highlight html %}

<ej-schedule id="Schedule" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings"></ej-schedule>

<script type="text/javascript">
$(function () {
    window.signalR = $.signalR.scheduleHub;
    window.signalR.client.modify = function (action, data) {
        $("#Schedule1").ejSchedule('instance').notifyChanges(action, data);
    };
    $.signalR.hub.start({ jsonp: true }).done(function () {
        window.actionComplete = function (args) {
            if (args.methodType != "public" && (args.type == "beforeAppointmentCreate" || args.type == "beforeAppointmentChange" || args.type == "beforeAppointmentRemove")) {
                window.signalR.server.modify(args.type, args.appointment);
            }
        };
    });
});
</script>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 12, 00),
                StartTimeZone: "UTC +00:00",
                EndTimeZone: "UTC +00:00"
            }],
            id: "Id",
            startTime: "StartTime",
            endTime: "EndTime",
            subject: "Subject",
            startTimeZone: "StartTimeZone",
            endTimeZone: "EndTimeZone"
        };
    }

}

{% endhighlight %}

## Events

### actionBegin
{:#events:actionbegin}

Triggers on the beginning of every action that starts within the Schedule.

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
            <td class="name">argument</td>
            <td class="type">Object</td>
            <td class="description">Event parameters when view change action starts:
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
                        <td class="name">currentDate</td>
                        <td class="type">Object</td>
                        <td class="description">Returns the current date value.</td>
                    </tr>
                    <tr>
                        <td class="name">cancel</td>
                        <td class="type">boolean</td>
                        <td class="description">Returns the cancel option value.</td>
                    </tr>
                    <tr>
                        <td class="name">currentView</td>
                        <td class="type">string</td>
                        <td class="description">Returns the current view value.</td>
                    </tr>
                    <tr>
                        <td class="name">model</td>
                        <td class="type"><ts ref="ej.Schedule.Model"/><span class="param-type">Object</span></td>
                        <td class="description">Returns the Schedule model.</td>
                    </tr>
                    <tr>
                        <td class="name">requestType</td>
                        <td class="type">string</td>
                        <td class="description">Returns the action begin request type.</td>
                    </tr>
                    <tr>
                        <td class="name">target</td>
                        <td class="type">Object</td>
                        <td class="description">Returns the target of the click.</td>
                    </tr>
                    <tr>
                        <td class="name">type</td>
                        <td class="type">string</td>
                        <td class="description">Returns the name of the event.</td>
                    </tr>
                </tbody>
                </table>
            </td>
        </tr>
        <tr>
            <td class="name">argument</td>
            <td class="type">Object</td>
            <td class="description">Event parameters when date navigate action starts:
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
                        <td class="name">currentDate</td>
                        <td class="type">Object</td>
                        <td class="description">Returns the current date value.</td>
                    </tr>
                    <tr>
                        <td class="name">model</td>
                        <td class="type"><ts ref="ej.Schedule.Model"/><span class="param-type">Object</span></td>
                        <td class="description">Returns the Schedule model.</td>
                    </tr>
                    <tr>
                        <td class="name">requestType</td>
                        <td class="type">string</td>
                        <td class="description">Returns the action begin request type.</td>
                    </tr>
                    <tr>
                        <td class="name">target</td>
                        <td class="type">Object</td>
                        <td class="description">Returns the target of the click.</td>
                    </tr>
                    <tr>
                        <td class="name">type</td>
                        <td class="type">string</td>
                        <td class="description">Returns the name of the event.</td>
                    </tr>
                </tbody>
            </table>
            </td>
        </tr>
        <tr>
            <td class="name">argument</td>
            <td class="type">Object</td>
            <td class="description">Event parameters when date changed through Scheduler calendar:
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
                        <td class="name">currentDate</td>
                        <td class="type">Object</td>
                        <td class="description">Returns the current date value.</td>
                    </tr>
                    <tr>
                        <td class="name">model</td>
                        <td class="type"><ts ref="ej.Schedule.Model"/><span class="param-type">Object</span></td>
                        <td class="description">Returns the Schedule model.</td>
                    </tr>
                    <tr>
                        <td class="name">requestType</td>
                        <td class="type">string</td>
                        <td class="description">Returns the action begin request type.</td>
                    </tr>
                    <tr>
                        <td class="name">target</td>
                        <td class="type">Object</td>
                        <td class="description">Returns the target of the click.</td>
                    </tr>
                    <tr>
                        <td class="name">type</td>
                        <td class="type">string</td>
                        <td class="description">Returns the name of the event.</td>
                    </tr>
                </tbody>
                </table>
            </td>
        </tr>
        <tr>
            <td class="name">argument</td>
            <td class="type">Object</td>
            <td class="description">Event parameters when appointment save action starts:
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
                            <td class="type">boolean</td>
                            <td class="description">Returns the cancel option value.</td>
                        </tr>
                        <tr>
                            <td class="name">data</td>
                            <td class="type">Object</td>
                            <td class="description">Returns the save appointment value.</td>
                        </tr>
                        <tr>
                            <td class="name">model</td>
                            <td class="type"><ts ref="ej.Schedule.Model"/><span class="param-type">Object</span></td>                          <td class="description">Returns the Schedule model.</td>
                        </tr>
                        <tr>
                            <td class="name">requestType</td>
                            <td class="type">string</td>
                            <td class="description">Returns the action begin request type.</td>
                        </tr>
                        <tr>
                            <td class="name">type</td>
                            <td class="type">string</td>
                            <td class="description">Returns the name of the event.</td>
                        </tr>
                    </tbody>
                </table>
            </td>
        </tr>
        <tr>
            <td class="name">argument</td>
            <td class="type">Object</td>
            <td class="description">Event parameters when appointment edit action starts:
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
                        <td class="name">data</td>
                        <td class="type">Object</td>
                        <td class="description">Returns the edit appointment value.</td>
                    </tr>
                    <tr>
                        <td class="name">model</td>
                        <td class="type"><ts ref="ej.Schedule.Model"/><span class="param-type">Object</span></td>
                        <td class="description">Returns the Schedule model.</td>
                    </tr>
                    <tr>
                        <td class="name">requestType</td>
                        <td class="type">string</td>
                        <td class="description">Returns the action begin request type.</td>
                    </tr>
                    <tr>
                        <td class="name">type</td>
                        <td class="type">string</td>
                        <td class="description">Returns the name of the event.</td>
                    </tr>
                </tbody>
             </table>
           </td>
        </tr>
        <tr>
            <td class="name">argument</td>
            <td class="type">Object</td>
            <td class="description">Event parameters when appointment delete action starts:
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
                        <td class="name">id</td>
                        <td class="type">number</td>
                        <td class="description">Returns the id of delete appointment.</td>
                    </tr>
                    <tr>
                        <td class="name">model</td>
                        <td class="type"><ts ref="ej.Schedule.Model"/><span class="param-type">Object</span></td>
                        <td class="description">Returns the Schedule model.</td>
                    </tr>
                    <tr>
                        <td class="name">requestType</td>
                        <td class="type">string</td>
                        <td class="description">Returns the action begin request type.</td>
                    </tr>
                    <tr>
                        <td class="name">type</td>
                        <td class="type">string</td>
                        <td class="description">Returns the name of the event.</td>
                    </tr>
                </tbody>
            </table>
            </td>
        </tr>
        <tr>
            <td class="name">argument</td>
            <td class="type">Object</td>
            <td class="description">Event parameters when appointment drag action starts:
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
                        <td class="name">data</td>
                        <td class="type">Object</td>
                        <td class="description">Returns the target of the appointment you drag.</td>
                    </tr>
                    <tr>
                        <td class="name">model</td>
                        <td class="type"><ts ref="ej.Schedule.Model"/><span class="param-type">Object</span></td>
                        <td class="description">Returns the Schedule model.</td>
                    </tr>
                    <tr>
                        <td class="name">requestType</td>
                        <td class="type">string</td>
                        <td class="description">Returns the action begin request type.</td>
                    </tr>
                    <tr>
                        <td class="name">type</td>
                        <td class="type">string</td>
                        <td class="description">Returns the name of the event.</td>
                    </tr>
                </tbody>
            </table>
            </td>
        </tr>
        <tr>
            <td class="name">argument</td>
            <td class="type">Object</td>
            <td class="description">Event parameters when appointment resize action starts:
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
                        <td class="type">boolean</td>
                        <td class="description">Returns the cancel option value.</td>
                    </tr>
                    <tr>
                        <td class="name">data</td>
                        <td class="type">Object</td>
                        <td class="description">Returns the target of the appointment you resize.</td>
                    </tr>
                    <tr>
                        <td class="name">model</td>
                        <td class="type"><ts ref="ej.Schedule.Model"/><span class="param-type">Object</span></td>
                        <td class="description">Returns the Schedule model.</td>
                    </tr>
                    <tr>
                        <td class="name">requestType</td>
                        <td class="type">string</td>
                        <td class="description">Returns the action begin request type.</td>
                    </tr>
                    <tr>
                        <td class="name">type</td>
                        <td class="type">string</td>
                        <td class="description">Returns the name of the event.</td>
                    </tr>
                </tbody>
            </table>
            </td>
         </tr>
    </tbody>
</table>

#### Example

{% highlight html %}

<ej-schedule id="Schedule" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings" (actionBegin)="onActionBegin($event)"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 12, 00),
                StartTimeZone: "UTC +00:00",
                EndTimeZone: "UTC +00:00"
            }],
            id: "Id",
            startTime: "StartTime",
            endTime: "EndTime",
            subject: "Subject",
            startTimeZone: "StartTimeZone",
            endTimeZone: "EndTimeZone"
        };
    }

    onActionBegin(args) {
        /* Do further actions here */
    }

}

{% endhighlight %}

### actionComplete
{:#events:actioncomplete}

Triggers after the completion of every action within the Schedule.

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
        <td class="name">argument</td>
        <td class="type">Object</td>
        <td class="description">Event parameters when view change action completes:
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
                    <td class="name">data</td>
                    <td class="type">Object</td>
                    <td class="description">Returns the data about view change action.</td>
                </tr>
                <tr>
                    <td class="name">model</td>
                    <td class="type"><ts ref="ej.Schedule.Model"/><span class="param-type">Object</span></td>
                    <td class="description">Returns the Schedule model.</td>
                </tr>
                <tr>
                    <td class="name">requestType</td>
                    <td class="type">string</td>
                    <td class="description">Returns the action complete request type.</td>
                </tr>
                <tr>
                    <td class="name">type</td>
                    <td class="type">string</td>
                    <td class="description">Returns the name of the event.</td>
                </tr>
            </tbody>
        </table>
        </td>
    </tr>
    <tr>
        <td class="name">argument</td>
        <td class="type">Object</td>
        <td class="description">Event parameters when date navigate action completes:
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
                    <td class="name">data</td>
                    <td class="type">Object</td>
                    <td class="description">Returns the data about the date navigate action.</td>
                </tr>
                <tr>
                    <td class="name">model</td>
                    <td class="type"><ts ref="ej.Schedule.Model"/><span class="param-type">Object</span></td>
                    <td class="description">Returns the Schedule model.</td>
                </tr>
                <tr>
                    <td class="name">requestType</td>
                    <td class="type">string</td>
                    <td class="description">Returns the action complete request type.</td>
                </tr>
                <tr>
                    <td class="name">type</td>
                    <td class="type">string</td>
                    <td class="description">Returns the name of the event.</td>
                </tr>
            </tbody>
        </table>
        </td>
    </tr>
    <tr>
        <td class="name">argument</td>
        <td class="type">Object</td>
        <td class="description">Event parameters when date change action through Scheduler calendar completes:
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
                    <td class="name">data</td>
                    <td class="type">Object</td>
                    <td class="description">Returns the data about calendar navigation action.</td>
                </tr>
                <tr>
                    <td class="name">model</td>
                    <td class="type"><ts ref="ej.Schedule.Model"/><span class="param-type">Object</span></td>
                    <td class="description">Returns the Schedule model.</td>
                </tr>
                <tr>
                    <td class="name">requestType</td>
                    <td class="type">string</td>
                    <td class="description">Returns the action complete request type.</td>
                </tr>
                <tr>
                    <td class="name">type</td>
                    <td class="type">string</td>
                    <td class="description">Returns the name of the event.</td>
                </tr>
            </tbody>
        </table>
        </td>
    </tr>
    <tr>
        <td class="name">argument</td>
        <td class="type">Object</td>
        <td class="description">Event parameters when appointment save action completes:
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
                    <td class="type">boolean</td>
                    <td class="description">Returns the cancel option value.</td>
                </tr>
                <tr>
                    <td class="name">data</td>
                    <td class="type">Object</td>
                    <td class="description">Returns the data about appointment saved value.</td>
                </tr>
                <tr>
                    <td class="name">model</td>
                    <td class="type"><ts ref="ej.Schedule.Model"/><span class="param-type">Object</span></td>
                    <td class="description">Returns the Schedule model.</td>
                </tr>
                <tr>
                    <td class="name">requestType</td>
                    <td class="type">string</td>
                    <td class="description">Returns the action complete request type.</td>
                </tr>
                <tr>
                    <td class="name">type</td>
                    <td class="type">string</td>
                    <td class="description">Returns the name of the event.</td>
                </tr>
            </tbody>
          </table>
        </td>
    </tr>
    <tr>
        <td class="name">argument</td>
        <td class="type">Object</td>
        <td class="description">Event parameters when appointment edit action completes:
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
                    <td class="type">boolean</td>
                    <td class="description">Returns the cancel option value.</td>
                </tr>
                <tr>
                    <td class="name">data</td>
                    <td class="type">Object</td>
                    <td class="description">Returns the data about appointment edited value.</td>
                </tr>
                <tr>
                    <td class="name">model</td>
                    <td class="type"><ts ref="ej.Schedule.Model"/><span class="param-type">Object</span></td>
                    <td class="description">Returns the Schedule model.</td>
                </tr>
                <tr>
                    <td class="name">requestType</td>
                    <td class="type">string</td>
                    <td class="description">Returns the action complete request type.</td>
                </tr>
                <tr>
                    <td class="name">type</td>
                    <td class="type">string</td>
                    <td class="description">Returns the name of the event.</td>
                </tr>
              </tbody>
            </table>
        </td>
    </tr>
    <tr>
        <td class="name">argument</td>
        <td class="type">Object</td>
        <td class="description">Event parameters when appointment delete action completes:
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
                    <td class="name">data</td>
                    <td class="type">Object</td>
                    <td class="description">Returns the data about appointment deleted action.</td>
                </tr>
                <tr>
                    <td class="name">model</td>
                    <td class="type"><ts ref="ej.Schedule.Model"/><span class="param-type">Object</span></td>
                    <td class="description">Returns the Schedule model.</td>
                </tr>
                <tr>
                    <td class="name">requestType</td>
                    <td class="type">string</td>
                    <td class="description">Returns the action complete request type.</td>
                </tr>
                <tr>
                    <td class="name">type</td>
                    <td class="type">string</td>
                    <td class="description">Returns the name of the event.</td>
                </tr>
            </tbody>
          </table>
        </td>
    </tr>
    <tr>
        <td class="name">argument</td>
        <td class="type">Object</td>
        <td class="description">Event parameters when appointment dragging action completes:
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
                    <td class="name">appointment</td>
                    <td class="type">Object</td>
                    <td class="description">Returns the appointment data dropped.</td>
                </tr>
                <tr>
                    <td class="name">cancel</td>
                    <td class="type">boolean</td>
                    <td class="description">Returns the cancel option value.</td>
                </tr>
                <tr>
                    <td class="name">model</td>
                    <td class="type"><ts ref="ej.Schedule.Model"/><span class="param-type">Object</span></td>
                    <td class="description">Returns the Schedule model.</td>
                </tr>
                <tr>
                    <td class="name">requestType</td>
                    <td class="type">string</td>
                    <td class="description">Returns the action complete request type.</td>
                </tr>
                <tr>
                    <td class="name">type</td>
                    <td class="type">string</td>
                    <td class="description">Returns the name of the event.</td>
                </tr>
             </tbody>
        </table>
        </td>
    </tr>
    <tr>
        <td class="name">argument</td>
        <td class="type">Object</td>
        <td class="description">Event parameters when appointment resizing action completes:
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
                    <td class="name">data</td>
                    <td class="type">Object</td>
                    <td class="description">Returns the element we resized.</td>
                </tr>
                <tr>
                    <td class="name">model</td>
                    <td class="type"><ts ref="ej.Schedule.Model"/><span class="param-type">Object</span></td>
                    <td class="description">Returns the Schedule model.</td>
                </tr>
                <tr>
                    <td class="name">requestType</td>
                    <td class="type">string</td>
                    <td class="description">Returns the action complete request type.</td>
                </tr>
                <tr>
                    <td class="name">type</td>
                    <td class="type">string</td>
                    <td class="description">Returns the name of the event.</td>
                </tr>
            </tbody>
        </table>
        </td>
    </tr>
    </tbody>
</table>

#### Example

{% highlight html %}

<ej-schedule id="Schedule" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings" (actionComplete)="onActionComplete($event)"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 12, 00),
                StartTimeZone: "UTC +00:00",
                EndTimeZone: "UTC +00:00"
            }],
            id: "Id",
            startTime: "StartTime",
            endTime: "EndTime",
            subject: "Subject",
            startTimeZone: "StartTimeZone",
            endTimeZone: "EndTimeZone"
        };
    }

    onActionComplete(args) {
        /* Do further actions here */
    }

}

{% endhighlight %}

### appointmentClick
{:#events:appointmentclick}

Triggers after an appointment is clicked.

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
            <td class="name">object</td>
            <td class="type">Object</td>
            <td class="description">Returns the object of appointmentClick event.</td>
        </tr>
        <tr>
            <td class="name">appointment</td>
            <td class="type">Object</td>
            <td class="description">Returns the clicked appointment object.</td>
        </tr>
        <tr>
            <td class="name">cancel</td>
            <td class="type">boolean</td>
            <td class="description">Returns the cancel option value.</td>
        </tr>
        <tr>
            <td class="name">model</td>
            <td class="type"><ts ref="ej.Schedule.Model"/><span class="param-type">Object</span></td>
            <td class="description">Returns the Schedule model.</td>
        </tr>
        <tr>
            <td class="name">type</td>
            <td class="type">string</td>
            <td class="description">Returns the name of the event.</td>
        </tr>
    </tbody>
</table>

#### Example

{% highlight html %}

<ej-schedule id="Schedule" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings" (appointmentClick)="onAppointmentClick($event)"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 12, 00),
                AllDay:true,
                Recurrence:false,
                RecurrenceRule:null,
                StartTimeZone: "UTC +00:00",
                EndTimeZone: "UTC +00:00"
            }],
            id: "Id",
            startTime: "StartTime",
            endTime: "EndTime",
            subject: "Subject",
            allDay:"AllDay",
            recurrence:"Recurrence",
            recurrenceRule:"RecurrenceRule",
            startTimeZone: "StartTimeZone",
            endTimeZone: "EndTimeZone"
        };
    }

    onAppointmentClick(args) {
        /* Do further actions here */
    }

}

{% endhighlight %}

### beforeAppointmentRemove
{:#events:beforeappointmentremove}


Triggers before the appointment is being removed from the Scheduler.

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
            <td class="name">appointment</td>
            <td class="type">Object</td>
            <td class="description">Returns the deleted appointment object.</td>
        </tr>
        <tr>
            <td class="name">model</td>
            <td class="type"><ts ref="ej.Schedule.Model"/><span class="param-type">Object</span></td>
            <td class="description">Returns the Schedule model.</td>
        </tr>
        <tr>
            <td class="name">type</td>
            <td class="type">string</td>
            <td class="description">Returns the name of the Scheduler event.</td>
        </tr>
    </tbody>
</table>

#### Example

{% highlight html %}

<ej-schedule id="Schedule" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings" (beforeAppointmentRemove)="onBeforeAppointmentRemove($event)"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 12, 00),
                StartTimeZone: "UTC +00:00",
                EndTimeZone: "UTC +00:00"
            }],
            id: "Id",
            startTime: "StartTime",
            endTime: "EndTime",
            subject: "Subject",
            startTimeZone: "StartTimeZone",
            endTimeZone: "EndTimeZone"
        };
    }

    onBeforeAppointmentRemove(args) {
        /* Do further actions here */
    }

}

{% endhighlight %}

### beforeAppointmentChange
{:#events:beforeappointmentchange}

Triggers before the edited appointment is being saved.

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
            <td class="name">appointment</td>
            <td class="type">Object</td>
            <td class="description">Returns the edited appointment object.</td>
        </tr>
        <tr>
            <td class="name">cancel</td>
            <td class="type">boolean</td>
            <td class="description">Returns the cancel option value.</td>
        </tr>
        <tr>
            <td class="name">model</td>
            <td class="type"><ts ref="ej.Schedule.Model"/><span class="param-type">Object</span></td>
            <td class="description">Returns the Schedule model.</td>
        </tr>
        <tr>
            <td class="name">type</td>
            <td class="type">string</td>
            <td class="description">Returns the name of the Scheduler event.</td>
        </tr>
    </tbody>
</table>

#### Example

{% highlight html %}

<ej-schedule id="Schedule" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings" (beforeAppointmentChange)="onBeforeAppointmentChange($event)"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 12, 00),
                StartTimeZone: "UTC +00:00",
                EndTimeZone: "UTC +00:00"
            }],
            id: "Id",
            startTime: "StartTime",
            endTime: "EndTime",
            subject: "Subject",
            startTimeZone: "StartTimeZone",
            endTimeZone: "EndTimeZone"
        };
    }

    onBeforeAppointmentChange(args) {
        /* Do further actions here */
    }

}

{% endhighlight %}

### appointmentHover
{:#events:appointmenthover}

Triggers on hovering the mouse over the appointments.

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
            <td class="name">object</td>
            <td class="type">Object</td>
            <td class="description">Returns the object of appointmentHover event.</td>
        </tr>
        <tr>
            <td class="name">appointment</td>
            <td class="type">Object</td>
            <td class="description">Returns the hovered appointment object.</td>
        </tr>
        <tr>
            <td class="name">cancel</td>
            <td class="type">boolean</td>
            <td class="description">Returns the cancel option value.</td>
        </tr>
        <tr>
            <td class="name">model</td>
            <td class="type"><ts ref="ej.Schedule.Model"/><span class="param-type">Object</span></td>
            <td class="description">Returns the Schedule model.</td>
        </tr>
        <tr>
            <td class="name">type</td>
            <td class="type">string</td>
            <td class="description">Returns the name of the event.</td>
        </tr>
    </tbody>
</table>

#### Example

{% highlight html %}

<ej-schedule id="Schedule" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings" (appointmentHover)="onAppointmentHover($event)"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 12, 00),
                StartTimeZone: "UTC +00:00",
                EndTimeZone: "UTC +00:00"
            }],
            id: "Id",
            startTime: "StartTime",
            endTime: "EndTime",
            subject: "Subject",
            startTimeZone: "StartTimeZone",
            endTimeZone: "EndTimeZone"
        };
    }

    onAppointmentHover(args) {
        /* Do further actions here */
    }

}

{% endhighlight %}

### beforeAppointmentCreate
{:#events:beforeappointmentcreate}

Triggers before the new appointment gets saved.

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
            <td class="name">appointment</td>
            <td class="type">Object</td>
            <td class="description">Returns the appointment object.</td>
        </tr>
        <tr>
            <td class="name">cancel</td>
            <td class="type">boolean</td>
            <td class="description">Returns the cancel option value.</td>
        </tr>
        <tr>
            <td class="name">model</td>
            <td class="type"><ts ref="ej.Schedule.Model"/><span class="param-type">Object</span></td>
            <td class="description">Returns the Schedule model.</td>
        </tr>
        <tr>
            <td class="name">type</td>
            <td class="type">string</td>
            <td class="description">Returns the name of the Scheduler event.</td>
        </tr>
    </tbody>
</table>

#### Example

{% highlight html %}

<ej-schedule id="Schedule" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings" (beforeAppointmentCreate)="onBeforeAppointmentCreate($event)"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 12, 00),
                StartTimeZone: "UTC +00:00",
                EndTimeZone: "UTC +00:00"
            }],
            id: "Id",
            startTime: "StartTime",
            endTime: "EndTime",
            subject: "Subject",
            startTimeZone: "StartTimeZone",
            endTimeZone: "EndTimeZone"
        };
    }

    onBeforeAppointmentCreate(args) {
        /* Do further actions here */
    }

}

{% endhighlight %}

### appointmentWindowOpen
{:#events:appointmentwindowopen}

Triggers before the appointment window opens.

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
            <td class="name">object</td>
            <td class="type">Object</td>
            <td class="description">returns the object of appointmentWindowOpen event while selecting the detail option from quick window or edit appointment or edit series option.</td>
        </tr>
        <tr>
            <td class="name">cancel</td>
            <td class="type">boolean</td>
            <td class="description">Returns the cancel option value.</td>
        </tr>
        <tr>
            <td class="name">endTime</td>
            <td class="type">Object</td>
            <td class="description">Returns the end time of the double clicked cell.</td>
        </tr>
        <tr>
            <td class="name">model</td>
            <td class="type"><ts ref="ej.Schedule.Model"/><span class="param-type">Object</span></td>
            <td class="description">Returns the Schedule model.</td>
        </tr>
        <tr>
            <td class="name">originalEventType</td>
            <td class="type">string</td>
            <td class="description">Returns the action name that triggers window open.</td>
        </tr>
        <tr>
            <td class="name">startTime</td>
            <td class="type">Object</td>
            <td class="description">Returns the start time of the double clicked cell.</td>
        </tr>
        <tr>
            <td class="name">target</td>
            <td class="type">Object</td>
            <td class="description">Returns the target of the double clicked cell.</td>
        </tr>
        <tr>
            <td class="name">type</td>
            <td class="type">string</td>
            <td class="description">Returns the name of the event.</td>
        </tr>
        <tr>
            <td class="name">appointment</td>
            <td class="type">Object</td>
            <td class="description">Returns the edit appointment object.</td>
        </tr>
        <tr>
            <td class="name">edit</td>
            <td class="type">boolean</td>
            <td class="description">Returns the edit occurrence option value.</td>
        </tr>
    </tbody>
</table>

#### Example

{% highlight html %}

<ej-schedule id="Schedule" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings" (appointmentWindowOpen)="onAppointmentWindowOpen($event)"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 12, 00),
                StartTimeZone: "UTC +00:00",
                EndTimeZone: "UTC +00:00"
            }],
            id: "Id",
            startTime: "StartTime",
            endTime: "EndTime",
            subject: "Subject",
            startTimeZone: "StartTimeZone",
            endTimeZone: "EndTimeZone"
        };
    }

    onAppointmentWindowOpen(args) {
        /* Do further actions here */
    }

}

{% endhighlight %}

### beforeContextMenuOpen
{:#events:beforecontextmenuopen}

Triggers before the context menu opens.

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
            <td class="name">object</td>
            <td class="type">Object</td>
            <td class="description">Returns the object of beforeContextMenuOpen event.</td>
        </tr>
        <tr>
            <td class="name">cancel</td>
            <td class="type">boolean</td>
            <td class="description">Returns the cancel option value.</td>
        </tr>
        <tr>
            <td class="name">cellIndex</td>
            <td class="type">number</td>
            <td class="description">Returns the current cell index value.</td>
        </tr>
        <tr>
            <td class="name">currentDate</td>
            <td class="type">Object</td>
            <td class="description">Returns the current date value.</td>
        </tr>
        <tr>
            <td class="name">resources</td>
            <td class="type">Object</td>
            <td class="description">Returns the current resource details, when multiple resources are present, otherwise returns null.</td>
        </tr>
        <tr>
            <td class="name">appointment</td>
            <td class="type">Object</td>
            <td class="description">Returns the current appointment details while opening the menu from appointment.</td>
        </tr>
        <tr>
            <td class="name">events</td>
            <td class="type">Object</td>
            <td class="description">Returns the object of before opening menu target.</td>
        </tr>
        <tr>
            <td class="name">model</td>
            <td class="type"><ts ref="ej.Schedule.Model"/><span class="param-type">Object</span></td>
            <td class="description">Returns the Schedule model.</td>
        </tr>
        <tr>
            <td class="name">type</td>
            <td class="type">string</td>
            <td class="description">Returns the name of the event.</td>
        </tr>
    </tbody>
</table>

#### Example

{% highlight html %}

<ej-schedule id="Schedule" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings" (beforeContextMenuOpen)="onBeforeContextMenuOpen($event)"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 12, 00),
                StartTimeZone: "UTC +00:00",
                EndTimeZone: "UTC +00:00"
            }],
            id: "Id",
            startTime: "StartTime",
            endTime: "EndTime",
            subject: "Subject",
            startTimeZone: "StartTimeZone",
            endTimeZone: "EndTimeZone"
        };
    }

    onBeforeContextMenuOpen(args) {
        /* Do further actions here */
    }

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
            <td class="name">object</td>
            <td class="type">Object</td>
            <td class="description">Returns the object of cellClick event.</td>
        </tr>
        <tr>
            <td class="name">cancel</td>
            <td class="type">boolean</td>
            <td class="description">Returns the cancel option value.</td>
        </tr>
        <tr>
            <td class="name">endTime</td>
            <td class="type">Object</td>
            <td class="description">Returns the end time of the clicked cell.</td>
        </tr>
        <tr>
            <td class="name">model</td>
            <td class="type"><ts ref="ej.Schedule.Model"/><span class="param-type">Object</span></td>
            <td class="description">Returns the Schedule model.</td>
        </tr>
        <tr>
            <td class="name">startTime</td>
            <td class="type">Object</td>
            <td class="description">Returns the start time of the clicked cell.</td>
        </tr>
        <tr>
            <td class="name">target</td>
            <td class="type">Object</td>
            <td class="description">Returns the target of the clicked cell.</td>
        </tr>
        <tr>
            <td class="name">type</td>
            <td class="type">string</td>
            <td class="description">Returns the name of the event.</td>
        </tr>
    </tbody>
</table>

#### Example

{% highlight html %}

<ej-schedule id="Schedule" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings" (cellClick)="onCellClick($event)"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 12, 00),
                StartTimeZone: "UTC +00:00",
                EndTimeZone: "UTC +00:00"
            }],
            id: "Id",
            startTime: "StartTime",
            endTime: "EndTime",
            subject: "Subject",
            startTimeZone: "StartTimeZone",
            endTimeZone: "EndTimeZone"
        };
    }

    onCellClick(args) {
        /* Do further actions here */
    }

}

{% endhighlight %}

### cellDoubleClick
{:#events:celldoubleclick}

Triggers after the cell is clicked twice.

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
            <td class="name">object</td>
            <td class="type">Object</td>
            <td class="description">Returns the object of cellDoubleClick event.</td>
        </tr>
        <tr>
            <td class="name">cancel</td>
            <td class="type">boolean</td>
            <td class="description">Returns the cancel option value.</td>
        </tr>
        <tr>
            <td class="name">endTime</td>
            <td class="type">Object</td>
            <td class="description">Returns the end time of the double clicked cell.</td>
        </tr>
        <tr>
            <td class="name">model</td>
            <td class="type"><ts ref="ej.Schedule.Model"/><span class="param-type">Object</span></td>
            <td class="description">Returns the Schedule model.</td>
        </tr>
        <tr>
            <td class="name">startTime</td>
            <td class="type">Object</td>
            <td class="description">Returns the start time of the double clicked cell.</td>
        </tr>
        <tr>
            <td class="name">target</td>
            <td class="type">Object</td>
            <td class="description">Returns the target of the double clicked cell.</td>
        </tr>
        <tr>
            <td class="name">type</td>
            <td class="type">string</td>
            <td class="description">Returns the name of the event.</td>
        </tr>
    </tbody>
</table>

#### Example

{% highlight html %}

<ej-schedule id="Schedule" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings" (cellDoubleClick)="onCellDoubleClick($event)"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 12, 00),
                StartTimeZone: "UTC +00:00",
                EndTimeZone: "UTC +00:00"
            }],
            id: "Id",
            startTime: "StartTime",
            endTime: "EndTime",
            subject: "Subject",
            startTimeZone: "StartTimeZone",
            endTimeZone: "EndTimeZone"
        };
    }

    onCellDoubleClick(args) {
        /* Do further actions here */
    }

}

{% endhighlight %}

### cellHover
{:#events:cellhover}

Triggers on hovering the mouse overs the cells.

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
            <td class="name">object</td>
            <td class="type">Object</td>
            <td class="description">Returns the object of cellHover event.</td>
        </tr>
        <tr>
            <td class="name">cancel</td>
            <td class="type">boolean</td>
            <td class="description">Returns the cancel option value.</td>
        </tr>
        <tr>
            <td class="name">cellIndex</td>
            <td class="type">Object</td>
            <td class="description">Returns the index of the hovered cell.</td>
        </tr>
        <tr>
            <td class="name">currentDate</td>
            <td class="type">Object</td>
            <td class="description">Returns the current date of the hovered cell.</td>
        </tr>
        <tr>
            <td class="name">model</td>
            <td class="type"><ts ref="ej.Schedule.Model"/><span class="param-type">Object</span></td>
            <td class="description">Returns the Schedule model.</td>
        </tr>
        <tr>
            <td class="name">target</td>
            <td class="type">Object</td>
            <td class="description">Returns the target of the clicked cell.</td>
        </tr>
        <tr>
            <td class="name">type</td>
            <td class="type">string</td>
            <td class="description">Returns the name of the event.</td>
        </tr>
    </tbody>
</table>

#### Example

{% highlight html %}

<ej-schedule id="Schedule" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings" (cellHover)="onCellHover($event)"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 12, 00),
                StartTimeZone: "UTC +00:00",
                EndTimeZone: "UTC +00:00"
            }],
            id: "Id",
            startTime: "StartTime",
            endTime: "EndTime",
            subject: "Subject",
            startTimeZone: "StartTimeZone",
            endTimeZone: "EndTimeZone"
        };
    }

    onCellHover(args) {
        /* Do further actions here */
    }

}

{% endhighlight %}

### create
{:#events:create}

Triggers when the Scheduler completely renders on the page.

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
            <td class="type"><ts ref="ej.Schedule.Model"/><span class="param-type">Object</span></td>
            <td class="description">Returns the Schedule model.</td>
        </tr>
        <tr>
            <td class="name">type</td>
            <td class="type">string</td>
            <td class="description">Returns the name of the Scheduler event.</td>
        </tr>
    </tbody>
</table>

#### Example

{% highlight html %}

<ej-schedule id="Schedule" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings" (create)="onCreate($event)"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 12, 00),
                StartTimeZone: "UTC +00:00",
                EndTimeZone: "UTC +00:00"
            }],
            id: "Id",
            startTime: "StartTime",
            endTime: "EndTime",
            subject: "Subject",
            startTimeZone: "StartTimeZone",
            endTimeZone: "EndTimeZone"
        };
    }

    onCreate(args) {
        /* Do further actions here */
    }

}

{% endhighlight %}

### destroy
{:#events:destroy}

Triggers when the Scheduler and all its sub-components gets destroyed.

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
            <td class="type"><ts ref="ej.Schedule.Model"/><span class="param-type">Object</span></td>
            <td class="description">Returns the Schedule model.</td>
        </tr>
        <tr>
            <td class="name">type</td>
            <td class="type">string</td>
            <td class="description">Returns the name of the Scheduler event.</td>
        </tr>
    </tbody>
</table>

#### Example

{% highlight html %}

<ej-schedule id="Schedule" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings" (destroy)="onDestroy($event)"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 12, 00),
                StartTimeZone: "UTC +00:00",
                EndTimeZone: "UTC +00:00"
            }],
            id: "Id",
            startTime: "StartTime",
            endTime: "EndTime",
            subject: "Subject",
            startTimeZone: "StartTimeZone",
            endTimeZone: "EndTimeZone"
        };
    }

    onDestroy(args) {
        /* Do further actions here */
    }

}

{% endhighlight %}

### drag
{:#events:drag}

Triggers while the appointment is being dragged over the work cells.

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
            <td class="name">object</td>
            <td class="type">Object</td>
            <td class="description">Returns the object of dragOver event.</td>
        </tr>
        <tr>
            <td class="name">cancel</td>
            <td class="type">boolean</td>
            <td class="description">Returns the cancel option value.</td>
        </tr>
        <tr>
            <td class="name">model</td>
            <td class="type"><ts ref="ej.Schedule.Model"/><span class="param-type">Object</span></td>
            <td class="description">Returns the Schedule model.</td>
        </tr>
        <tr>
            <td class="name">target</td>
            <td class="type">Object</td>
            <td class="description">Returns the target of the drag over appointment.</td>
        </tr>
        <tr>
            <td class="name">type</td>
            <td class="type">string</td>
            <td class="description">Returns the name of the event.</td>
        </tr>
    </tbody>
</table>

#### Example

{% highlight html %}

<ej-schedule id="Schedule" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings" (drag)="onDrag($event)"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 12, 00),
                StartTimeZone: "UTC +00:00",
                EndTimeZone: "UTC +00:00"
            }],
            id: "Id",
            startTime: "StartTime",
            endTime: "EndTime",
            subject: "Subject",
            startTimeZone: "StartTimeZone",
            endTimeZone: "EndTimeZone"
        };
    }

    onDrag(args) {
        /* Do further actions here */
    }

}

{% endhighlight %}

### dragStart
{:#events:dragstart}

Triggers when the appointment dragging begins.

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
            <td class="name">object</td>
            <td class="type">Object</td>
            <td class="description">Returns the object of dragStart event.</td>
        </tr>
        <tr>
            <td class="name">cancel</td>
            <td class="type">boolean</td>
            <td class="description">Returns the cancel option value.</td>
        </tr>
        <tr>
            <td class="name">model</td>
            <td class="type"><ts ref="ej.Schedule.Model"/><span class="param-type">Object</span></td>
            <td class="description">Returns the Schedule model.</td>
        </tr>
        <tr>
            <td class="name">target</td>
            <td class="type">Object</td>
            <td class="description">Returns the target of the dragging appointment.</td>
        </tr>
        <tr>
            <td class="name">type</td>
            <td class="type">string</td>
            <td class="description">Returns the name of the event.</td>
        </tr>
    </tbody>
</table>

Example
{:.example}

{% highlight html %}

<ej-schedule id="Schedule" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings" (dragStart)="onDragStart($event)"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 12, 00),
                StartTimeZone: "UTC +00:00",
                EndTimeZone: "UTC +00:00"
            }],
            id: "Id",
            startTime: "StartTime",
            endTime: "EndTime",
            subject: "Subject",
            startTimeZone: "StartTimeZone",
            endTimeZone: "EndTimeZone"
        };
    }

    onDragStart(args) {
        /* Do further actions here */
    }

}

{% endhighlight %}

### dragStop
{:#events:dragstop}

Triggers when the appointment is dropped.

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
            <td class="name">object</td>
            <td class="type">Object</td>
            <td class="description">Returns the object of dragDrop event.</td>
        </tr>
        <tr>
            <td class="name">appointment</td>
            <td class="type">Object</td>
            <td class="description">Returns the dropped appointment object.</td>
        </tr>
        <tr>
            <td class="name">cancel</td>
            <td class="type">boolean</td>
            <td class="description">Returns the cancel option value.</td>
        </tr>
        <tr>
            <td class="name">model</td>
            <td class="type"><ts ref="ej.Schedule.Model"/><span class="param-type">Object</span></td>
            <td class="description">Returns the Schedule model.</td>
        </tr>
        <tr>
            <td class="name">type</td>
            <td class="type">string</td>
            <td class="description">Returns the name of the event.</td>
        </tr>
    </tbody>
</table>

#### Example

{% highlight html %}

<ej-schedule id="Schedule" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings" (dragStop)="onDragStop($event)"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 12, 00),
                StartTimeZone: "UTC +00:00",
                EndTimeZone: "UTC +00:00"
            }],
            id: "Id",
            startTime: "StartTime",
            endTime: "EndTime",
            subject: "Subject",
            startTimeZone: "StartTimeZone",
            endTimeZone: "EndTimeZone"
        };
    }

    onDragStop(args) {
        /* Do further actions here */
    }

}

{% endhighlight %}

### menuItemClick
{:#events:menuitemclick}

Triggers after the menu/sub-menu items within the context menu is clicked.

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
            <td class="name">object</td>
            <td class="type">Object</td>
            <td class="description">Returns the object of menuItemClick event.</td>
        </tr>
        <tr>
            <td class="name">cancel</td>
            <td class="type">boolean</td>
            <td class="description">Returns the cancel option value.</td>
        </tr>
        <tr>
            <td class="name">events</td>
            <td class="type">Object</td>
            <td class="description">Returns the object of menu item event.</td>
        </tr>
        <tr>
            <td class="name">model</td>
            <td class="type"><ts ref="ej.Schedule.Model"/><span class="param-type">Object</span></td>
            <td class="description">Returns the Schedule model.</td>
        </tr>
        <tr>
            <td class="name">type</td>
            <td class="type">string</td>
            <td class="description">Returns the name of the event.</td>
        </tr>
    </tbody>
</table>

#### Example

{% highlight html %}

<ej-schedule id="Schedule" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings" (menuItemClick)="onMenuItemClick($event)"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 12, 00),
                StartTimeZone: "UTC +00:00",
                EndTimeZone: "UTC +00:00"
            }],
            id: "Id",
            startTime: "StartTime",
            endTime: "EndTime",
            subject: "Subject",
            startTimeZone: "StartTimeZone",
            endTimeZone: "EndTimeZone"
        };
    }

    onMenuItemClick(args) {
        /* Do further actions here */
    }

}

{% endhighlight %}

### navigation
{:#events:navigation}

Triggers after the Schedule view or date is navigated.

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
            <td class="name">argument</td>
            <td class="type">Object</td>
            <td class="description">Event parameters when view changes:
            Returns the object of Schedule view navigation event.
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
                        <td class="name">currentDate</td>
                        <td class="type">Object</td>
                        <td class="description">Returns the current date object.</td>
                    </tr>
                    <tr>
                        <td class="name">cancel</td>
                        <td class="type">boolean</td>
                        <td class="description">Returns the cancel option value.</td>
                    </tr>
                    <tr>
                        <td class="name">model</td>
                        <td class="type"><ts ref="ej.Schedule.Model"/><span class="param-type">Object</span></td>
                        <td class="description">Returns the Schedule model.</td>
                    </tr>
                    <tr>
                        <td class="name">currentView</td>
                        <td class="type">string</td>
                        <td class="description">Returns the current view value.</td>
                    </tr>
                    <tr>
                        <td class="name">previousView</td>
                        <td class="type">string</td>
                        <td class="description">Returns the previous view value.</td>
                    </tr>
                    <tr>
                        <td class="name">target</td>
                        <td class="type">Object</td>
                        <td class="description">Returns the target of the action.</td>
                    </tr>
                    <tr>
                        <td class="name">type</td>
                        <td class="type">string</td>
                        <td class="description">Returns the name of the event.</td>
                    </tr>
                </tbody>
            </table>
            </td>
        </tr>
        <tr>
            <td class="name">argument</td>
            <td class="type">Object</td>
            <td class="description">Returns the object of previous or next date navigation event:
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
                        <td class="type"><ts ref="ej.Schedule.Model"/><span class="param-type">Object</span></td>
                        <td class="description">Returns the Schedule model.</td>
                    </tr>
                    <tr>
                        <td class="name">currentDate</td>
                        <td class="type">Object</td>
                        <td class="description">Returns the new date of the Schedule.</td>
                    </tr>
                    <tr>
                        <td class="name">previousDate</td>
                        <td class="type">Object</td>
                        <td class="description">Returns the previous date of the Schedule.</td>
                    </tr>
                    <tr>
                        <td class="name">target</td>
                        <td class="type">Object</td>
                        <td class="description">Returns the target of the action.</td>
                    </tr>
                    <tr>
                        <td class="name">type</td>
                        <td class="type">string</td>
                        <td class="description">Returns the name of the event.</td>
                    </tr>
                </tbody>
            </table>
            </td>
        </tr>
        <tr>
            <td class="name">argument</td>
            <td class="type">Object</td>
            <td class="description">Returns the navigation event while changing the date by using calendar in Schedule.
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
                        <td class="type"><ts ref="ej.Schedule.Model"/><span class="param-type">Object</span></td>
                        <td class="description">Returns the Schedule model.</td>
                    </tr>
                    <tr>
                        <td class="name">currentDate</td>
                        <td class="type">Object</td>
                        <td class="description">Returns the new date of the Schedule.</td>
                    </tr>
                    <tr>
                        <td class="name">previousDate</td>
                        <td class="type">Object</td>
                        <td class="description">Returns the previous date of the Schedule.</td>
                    </tr>
                    <tr>
                        <td class="name">target</td>
                        <td class="type">Object</td>
                        <td class="description">Returns the target of the action.</td>
                    </tr>
                    <tr>
                        <td class="name">type</td>
                        <td class="type">string</td>
                        <td class="description">Returns the name of the event.</td> 
                    </tr>
                </tbody>
            </table>
            </td>
        </tr>
    </tbody>
</table>

#### Example

{% highlight html %}

<ej-schedule id="Schedule" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings" (navigation)="onNavigation($event)"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 12, 00),
                StartTimeZone: "UTC +00:00",
                EndTimeZone: "UTC +00:00"
            }],
            id: "Id",
            startTime: "StartTime",
            endTime: "EndTime",
            subject: "Subject",
            startTimeZone: "StartTimeZone",
            endTimeZone: "EndTimeZone"
        };
    }

    onNavigation(args) {
        /* Do further actions here */
    }

}

{% endhighlight %}

### queryCellInfo
{:#events:querycellinfo}

Triggers every time before the elements of the scheduler such as work cells, time cells or header cells and so on renders or re-renders on a page.

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
            <td class="type"><ts ref="ej.Schedule.Model"/><span class="param-type">Object</span></td>
            <td class="description">Returns the Schedule model.</td>
        </tr>
        <tr>
            <td class="name">appointment</td>
            <td class="type">Object</td>
            <td class="description">Returns the current appointment data.</td>
        </tr>
        <tr>
            <td class="name">element</td>
            <td class="type">Object</td>
            <td class="description">Returns the currently rendering DOM element.</td>
        </tr>
        <tr>
            <td class="name">requestType</td>
            <td class="type">string</td>
            <td class="description">Returns the name of the currently rendering element on the scheduler.</td>
        </tr>
        <tr>
            <td class="name">cellType</td>
            <td class="type">string</td>
            <td class="description">Returns the cell type which is currently rendering on the Scheduler.</td>
        </tr>
        <tr>
            <td class="name">currentAppointmentDate</td>
            <td class="type">Object</td>
            <td class="description">Returns the start date of the currently rendering appointment.</td>
        </tr>
        <tr>
            <td class="name">cell</td>
            <td class="type">Object</td>
            <td class="description">Returns the currently rendering cell information.</td>
        </tr>
        <tr>
            <td class="name">resource</td>
            <td class="type">Object</td>
            <td class="description">Returns the currently rendering resource details.</td>
        </tr>
        <tr>
            <td class="name">currentDay</td>
            <td class="type">Object</td>
            <td class="description">Returns the currently rendering date information.</td>
        </tr>
    </tbody>
</table>

#### Example

{% highlight html %}

<ej-schedule id="Schedule" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings" (queryCellInfo)="onQueryCellInfo($event)"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 12, 00),
                StartTimeZone: "UTC +00:00",
                EndTimeZone: "UTC +00:00"
            }],
            id: "Id",
            startTime: "StartTime",
            endTime: "EndTime",
            subject: "Subject",
            startTimeZone: "StartTimeZone",
            endTimeZone: "EndTimeZone"
        };
    }

    onQueryCellInfo(args) {
        switch (args.requestType) {
            case "workcells":
                args.element.css("background-color", "#dcf1f8");
                break;
            case "monthcells":
                args.element.css("background-color", "#dcf1f8");
                break;
            case "alldaycells":
                args.element.css("background-color", "#dcf1f8");
                break;
        }
    }

}

{% endhighlight %}

### reminder
{:#events:reminder}

Triggers when the reminder is raised for an appointment based on the `alertBefore` value.

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
            <td class="type"><ts ref="ej.Schedule.Model"/><span class="param-type">Object</span></td>
            <td class="description">Returns the Schedule model.</td>
        </tr>
        <tr>
            <td class="name">type</td>
            <td class="type">string</td>
            <td class="description">Returns the name of the event.</td>
        </tr>
        <tr>
            <td class="name">reminderAppointment</td>
            <td class="type">Object</td>
            <td class="description">Returns the appointment object for which the reminder is raised.</td>
        </tr>
    </tbody>
</table>

#### Example

{% highlight html %}

<ej-schedule id="Schedule" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings" (reminder)="onReminder($event)"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 12, 00),
                StartTimeZone: "UTC +00:00",
                EndTimeZone: "UTC +00:00"
            }],
            id: "Id",
            startTime: "StartTime",
            endTime: "EndTime",
            subject: "Subject",
            startTimeZone: "StartTimeZone",
            endTimeZone: "EndTimeZone"
        };
    }

    onReminder(args) {
        /* Do further actions here */
    }

}

{% endhighlight %}

### resize
{:#events:resize}

Triggers while resizing the appointment.

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
            <td class="name">object</td>
            <td class="type">Object</td>
            <td class="description">Returns the object of resizing event.</td>
        </tr>
        <tr>
            <td class="name">cancel</td>
            <td class="type">boolean</td>
            <td class="description">Returns the cancel option value.</td>
        </tr>
        <tr>
            <td class="name">element</td>
            <td class="type">Object</td>
            <td class="description">Returns the resize element value.</td>
        </tr>
        <tr>
            <td class="name">model</td>
            <td class="type"><ts ref="ej.Schedule.Model"/><span class="param-type">Object</span></td>
            <td class="description">Returns the Schedule model.</td>
        </tr>
        <tr>
            <td class="name">type</td>
            <td class="type">string</td>
            <td class="description">Returns the name of the event.</td>
        </tr>
    </tbody>
</table>

#### Example

{% highlight html %}

<ej-schedule id="Schedule" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings" (resize)="onResize($event)"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 12, 00),
                StartTimeZone: "UTC +00:00",
                EndTimeZone: "UTC +00:00"
            }],
            id: "Id",
            startTime: "StartTime",
            endTime: "EndTime",
            subject: "Subject",
            startTimeZone: "StartTimeZone",
            endTimeZone: "EndTimeZone"
        };
    }

    onResize(args) {
        /* Do further actions here */
    }

}

{% endhighlight %}

### resizeStart
{:#events:resizestart}

Triggers when the appointment resizing begins.

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
            <td class="name">object</td>
            <td class="type">Object</td>
            <td class="description">Returns the object of resizeStart event.</td>
        </tr>
        <tr>
            <td class="name">cancel</td>
            <td class="type">boolean</td>
            <td class="description">Returns the cancel option value.</td>
        </tr>
        <tr>
            <td class="name">element</td>
            <td class="type">Object</td>
            <td class="description">Returns the resize element value.</td>
        </tr>
        <tr>
            <td class="name">model</td>
            <td class="type"><ts ref="ej.Schedule.Model"/><span class="param-type">Object</span></td>
            <td class="description">Returns the Schedule model.</td>
        </tr>
        <tr>
            <td class="name">type</td>
            <td class="type">string</td>
            <td class="description">Returns the name of the event.</td>
        </tr>
    </tbody>
</table>

#### Example

{% highlight html %}

<ej-schedule id="Schedule" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings" (resizeStart)="onResizeStart($event)"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 12, 00),
                StartTimeZone: "UTC +00:00",
                EndTimeZone: "UTC +00:00"
            }],
            id: "Id",
            startTime: "StartTime",
            endTime: "EndTime",
            subject: "Subject",
            startTimeZone: "StartTimeZone",
            endTimeZone: "EndTimeZone"
        };
    }

    onResizeStart(args) {
        /* Do further actions here */
    }

}

{% endhighlight %}

### resizeStop
{:#events:resizestop}

Triggers when an appointment resizing stops.

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
            <td class="name">object</td>
            <td class="type">Object</td>
            <td class="description">Returns the object of resizeStop event.</td>
        </tr>
        <tr>
            <td class="name">appointment</td>
            <td class="type">Object</td>
            <td class="description">Returns the resized appointment value.</td>
        </tr>
        <tr>
            <td class="name">cancel</td>
            <td class="type">boolean</td>
            <td class="description">Returns the cancel option value.</td>
        </tr>
        <tr>
            <td class="name">model</td>
            <td class="type"><ts ref="ej.Schedule.Model"/><span class="param-type">Object</span></td>
            <td class="description">Returns the Schedule model.</td>
        </tr>
        <tr>
            <td class="name">target</td>
            <td class="type">Object</td>
            <td class="description">Returns the target of the resized appointment.</td>
        </tr>
        <tr>
            <td class="name">type</td>
            <td class="type">string</td>
            <td class="description">Returns the name of the event.</td>
        </tr>
    </tbody>
</table>

#### Example

{% highlight html %}

<ej-schedule id="Schedule" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings" (resizeStop)="onResizeStop($event)"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 12, 00),
                StartTimeZone: "UTC +00:00",
                EndTimeZone: "UTC +00:00"
            }],
            id: "Id",
            startTime: "StartTime",
            endTime: "EndTime",
            subject: "Subject",
            startTimeZone: "StartTimeZone",
            endTimeZone: "EndTimeZone"
        };
    }

    onResizeStop(args) {
        /* Do further actions here */
    }

}

{% endhighlight %}

### overflowButtonClick
{:#events:overflowbuttonclick}

Triggers when the overflow button is clicked.

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
            <td class="name">object</td>
            <td class="type">Object</td>
            <td class="description">Returns the object consisting of start time, end time and resource value of the underlying cell on which the clicked overflow button is present.  </td>
        </tr>
        <tr>
            <td class="name">cancel</td>
            <td class="type">boolean</td>
            <td class="description">Returns the cancel option value.</td>
        </tr>
        <tr>
            <td class="name">events</td>
            <td class="type">Object</td>
            <td class="description">Returns the object of menu item event.</td>
        </tr>
        <tr>
            <td class="name">model</td>
            <td class="type"><ts ref="ej.Schedule.Model"/><span class="param-type">Object</span></td>
            <td class="description">Returns the Schedule model.</td>
        </tr>
        <tr>
            <td class="name">type</td>
            <td class="type">string</td>
            <td class="description">Returns the name of the event.</td>
        </tr>
    </tbody>
</table>

#### Example

{% highlight html %}

<ej-schedule id="Schedule" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings" (overflowButtonClick)="onOverflowButtonClick($event)"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 12, 00),
                StartTimeZone: "UTC +00:00",
                EndTimeZone: "UTC +00:00"
            }],
            id: "Id",
            startTime: "StartTime",
            endTime: "EndTime",
            subject: "Subject",
            startTimeZone: "StartTimeZone",
            endTimeZone: "EndTimeZone"
        };
    }

    onOverflowButtonClick(args) {
        /* Do further actions here */
    }

}

{% endhighlight %}

### overflowButtonHover
{:#events:overflowbuttonhover}

Triggers while mouse hovering on the overflow button.

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
            <td class="name">object</td>
            <td class="type">Object</td>
            <td class="description">Returns the object consisting of start time, end time and resource value of the underlying cell on which the overflow button is currently hovered.  </td>
        </tr>
        <tr>
            <td class="name">cancel</td>
            <td class="type">boolean</td>
            <td class="description">Returns the cancel option value.</td>
        </tr>
        <tr>
            <td class="name">events</td>
            <td class="type">Object</td>
            <td class="description">Returns the object of menu item event.</td>
        </tr>
        <tr>
            <td class="name">model</td>
            <td class="type"><ts ref="ej.Schedule.Model"/><span class="param-type">Object</span></td>
            <td class="description">Returns the Schedule model.</td>
        </tr>
        <tr>
            <td class="name">type</td>
            <td class="type">string</td>
            <td class="description">Returns the name of the event.</td>
        </tr>
    </tbody>
</table>

#### Example

{% highlight html %}

<ej-schedule id="Schedule" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings" (overflowButtonHover)="onOverflowButtonHover($event)"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 12, 00),
                StartTimeZone: "UTC +00:00",
                EndTimeZone: "UTC +00:00"
            }],
            id: "Id",
            startTime: "StartTime",
            endTime: "EndTime",
            subject: "Subject",
            startTimeZone: "StartTimeZone",
            endTimeZone: "EndTimeZone"
        };
    }

    onOverflowButtonHover(args) {
        /* Do further actions here */
    }

}

{% endhighlight %}

### keyDown
{:#events:keydown}

Triggers when any of the keyboard keys are pressed.

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
            <td class="name">events</td>
            <td class="type">Object</td>
            <td class="description">Returns the object of menu item event.</td>
        </tr>
        <tr>
            <td class="name">model</td>
            <td class="type"><ts ref="ej.Schedule.Model"/><span class="param-type">Object</span></td>
            <td class="description">Returns the Schedule model.</td>
        </tr>
        <tr>
            <td class="name">type</td>
            <td class="type">string</td>
            <td class="description">Returns the name of the event.</td>
        </tr>
    </tbody>
</table>

#### Example

{% highlight html %}

<ej-schedule id="Schedule" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings" (keyDown)="onKeyDown($event)"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 12, 00),
                StartTimeZone: "UTC +00:00",
                EndTimeZone: "UTC +00:00"
            }],
            id: "Id",
            startTime: "StartTime",
            endTime: "EndTime",
            subject: "Subject",
            startTimeZone: "StartTimeZone",
            endTimeZone: "EndTimeZone"
        };
    }

    onKeyDown(args) {
        /* Do further actions here */
    }

}

{% endhighlight %}

### appointmentCreated
{:#events:appointmentcreated}

Triggers after the new appointment is saved.

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
            <td class="name">appointment</td>
            <td class="type">Object</td>
            <td class="description">Returns the appointment object.</td>
        </tr>
        <tr>
            <td class="name">cancel</td>
            <td class="type">boolean</td>
            <td class="description">Returns the cancel option value.</td>
        </tr>
        <tr>
            <td class="name">model</td>
            <td class="type"><ts ref="ej.Schedule.Model"/><span class="param-type">Object</span></td>
            <td class="description">Returns the Schedule model.</td>
        </tr>
        <tr>
            <td class="name">type</td>
            <td class="type">string</td>
            <td class="description">Returns the name of the Scheduler event.</td>
        </tr>
    </tbody>
</table>

#### Example

{% highlight html %}

<ej-schedule id="Schedule" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings" (appointmentCreated)="onAppointmentCreated($event)"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 12, 00),
                StartTimeZone: "UTC +00:00",
                EndTimeZone: "UTC +00:00"
            }],
            id: "Id",
            startTime: "StartTime",
            endTime: "EndTime",
            subject: "Subject",
            startTimeZone: "StartTimeZone",
            endTimeZone: "EndTimeZone"
        };
    }

    onAppointmentCreated(args) {
        /* Do further actions here */
    }

}

{% endhighlight %}

### appointmentChanged
{:#events:appointmentchanged}

Triggers after an existing appointment is edited.

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
            <td class="name">appointment</td>
            <td class="type">Object</td>
            <td class="description">Returns the edited appointment object.</td>
        </tr>
        <tr>
            <td class="name">cancel</td>
            <td class="type">boolean</td>
            <td class="description">Returns the cancel option value.</td>
        </tr>
        <tr>
            <td class="name">model</td>
            <td class="type"><ts ref="ej.Schedule.Model"/><span class="param-type">Object</span></td>
            <td class="description">Returns the Schedule model.</td>
        </tr>
        <tr>
            <td class="name">type</td>
            <td class="type">string</td>
            <td class="description">Returns the name of the Scheduler event.</td>
        </tr>
    </tbody>
</table>

#### Example

{% highlight html %}

<ej-schedule id="Schedule" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings" (appointmentChanged)="onAppointmentChanged($event)"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 12, 00),
                StartTimeZone: "UTC +00:00",
                EndTimeZone: "UTC +00:00"
            }],
            id: "Id",
            startTime: "StartTime",
            endTime: "EndTime",
            subject: "Subject",
            startTimeZone: "StartTimeZone",
            endTimeZone: "EndTimeZone"
        };
    }

    onAppointmentChanged(args) {
        /* Do further actions here */
    }

}

{% endhighlight %}

### appointmentRemoved
{:#events:appointmentremoved}

Triggers after the appointment is deleted.

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
            <td class="name">appointment</td>
            <td class="type">Object</td>
            <td class="description">Returns the deleted appointment object.</td>
        </tr>
        <tr>
            <td class="name">model</td>
            <td class="type"><ts ref="ej.Schedule.Model"/><span class="param-type">Object</span></td>
            <td class="description">Returns the Schedule model.</td>
        </tr>
        <tr>
            <td class="name">type</td>
            <td class="type">string</td>
            <td class="description">Returns the name of the Scheduler event.</td>
        </tr>
    </tbody>
</table>

#### Example

{% highlight html %}

<ej-schedule id="Schedule" [currentDate]="CurrentDate" [appointmentSettings]="AppointmentSettings" (appointmentRemoved)="onAppointmentRemoved($event)"></ej-schedule>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    public CurrentDate: date;
    public AppointmentSettings: any;
    constructor() {
        this.CurrentDate = new Date(2014, 4, 5);
        this.AppointmentSettings = {
            dataSource: [{
                Id: 101,
                Subject: "Talk with Nature",
                StartTime: new Date(2014, 4, 5, 10, 00),
                EndTime: new Date(2014, 4, 5, 12, 00),
                StartTimeZone: "UTC +00:00",
                EndTimeZone: "UTC +00:00"
            }],
            id: "Id",
            startTime: "StartTime",
            endTime: "EndTime",
            subject: "Subject",
            startTimeZone: "StartTimeZone",
            endTimeZone: "EndTimeZone"
        };
    }

    onAppointmentRemoved(args) {
        /* Do further actions here */
    }

}

{% endhighlight %}
