---
layout: post
title: Properties, Methods and Events of ejUploadbox Widget
description: API reference for ejUploadbox
documentation: API
platform: angular-api
keywords: Uploadbox, ejUploadbox, syncfusion, Uploadbox api 
---

# ejUploadbox





The Uploadbox control supports uploading files into the designated server, regardless of the file format and size. The Uploadbox control helps you with the selection of files to upload to the server. 





















#### Example








#### Requires



* module:jQuery


* module:jquery.easing.1.3.min.js


* module:ej.core.js


* module:ej.uploadbox.js


* module:ej.dialog.js


* module:ej.scroller.js


* module:ej.draggable.js




## Members








### allowDragAndDrop `boolean`
{:#members:allowdraganddrop}








Enables the file drag and drop support to the Uploadbox control.




#### Default Value







* false








#### Example

{% highlight html %}

<div id="upload_controls" style="margin-left: 35%;">
<div>Select a file to upload</div>
<div style="width:100px;height:35px;">
    <ej-uploadbox id="uploadDefault" [allowDragAndDrop]=true [saveUrl]="saveURL" [removeUrl]="removeURL"></ej-uploadbox>
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
  saveURL: string;
  removeURL: string;
  constructor() {
  this.saveURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Save';
  this.removeURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Remove';
  }
}


{% endhighlight %}







### asyncUpload `boolean`
{:#members:asyncupload}








Uploadbox supports both synchronous and asynchronous upload. This can be achieved by using the asyncUpload property.

Synchronous Upload -
Selected files are sent to the application form post action.	

Asynchronous Upload -
Selected files are sent to the server handler by using the AJAX Post.




#### Default Value







* true








#### Example

{% highlight html %}

<div id="upload_controls" style="margin-left: 35%;">
<div>Select a file to upload</div>
<div style="width:100px;height:35px;">
    <ej-uploadbox id="uploadDefault" [asyncUpload]=false [saveUrl]="saveURL" [removeUrl]="removeURL"></ej-uploadbox>
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
  saveURL: string;
  removeURL: string;
  constructor() {
  this.saveURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Save';
  this.removeURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Remove';
  }
}


{% endhighlight %}








### autoUpload `boolean`
{:#members:autoupload}








Uploadbox supports auto uploading of files after the file selection is done.




#### Default Value







* false








#### Example

{% highlight html %}

<div id="upload_controls" style="margin-left: 35%;">
<div>Select a file to upload</div>
<div style="width:100px;height:35px;">
    <ej-uploadbox id="uploadDefault" [autoUpload]=true [saveUrl]="saveURL" [removeUrl]="removeURL"></ej-uploadbox>
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
  saveURL: string;
  removeURL: string;
  constructor() {
  this.saveURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Save';
  this.removeURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Remove';
  }
}


{% endhighlight %}







### buttonText `object`
{:#members:buttontext}








Sets the text for each action button.




#### Default Value







* {browse: "Browse", upload: "Upload", cancel: "Cancel", close: "Close"}








#### Example

{% highlight html %}

<div id="upload_controls" style="margin-left: 35%;">
<div>Select a file to upload</div>
<div style="width:100px;height:35px;">
    <ej-uploadbox id="uploadDefault" [buttonText]="buttonText" [saveUrl]="saveURL" [removeUrl]="removeURL"></ej-uploadbox>
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
  saveURL: string;
  removeURL: string;
  buttonText: any;
  constructor() {
  this.saveURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Save';
  this.removeURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Remove';
  this.buttonText= { browse: "Choose File", upload: "Upload the File", cancel: "Cancel the Upload",close: "close the dialog"};
  }
}


{% endhighlight %}








### buttonText.browse `string`
{:#members:buttontext-browse}








Sets the text for the browse button.














### buttonText.cancel `string`
{:#members:buttontext-cancel}








Sets the text for the cancel button.













### buttonText.Close `string`
{:#members:buttontext-close}








Sets the text for the close button.













### buttonText.upload `string`
{:#members:buttontext-upload}








Sets the text for the Upload button inside the dialog popup.












### cssClass `string`
{:#members:cssclass}








Sets the root class for the Uploadbox control theme. This cssClass API helps to use custom skinning option for the Uploadbox button and dialog content.





#### Default Value







* ""








#### Example

{% highlight html %}

<div id="upload_controls" style="margin-left: 35%;">
<div>Select a file to upload</div>
<div style="width:100px;height:35px;">
    <ej-uploadbox id="uploadDefault" [saveUrl]="saveURL" cssClass="cssclass" [removeUrl]="removeURL"></ej-uploadbox>
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
  saveURL: string;
  removeURL: string;
  
  constructor() {
  this.saveURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Save';
  this.removeURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Remove';
  
  }
}


{% endhighlight %}

The css must be in stylesheet.

{% highlight html %}
<style>
.cssclass{

}
</style>
{% endhighlight %}








### customFileDetails `object`
{:#members:customfiledetails}








Specifies the custom file details in the dialog popup on initialization.




#### Default Value







* { title:true, name:true, size:true, status:true, action:true}








#### Example

{% highlight html %}

<div id="upload_controls" style="margin-left: 35%;">
<div>Select a file to upload</div>
<div style="width:100px;height:35px;">
    <ej-uploadbox id="uploadDefault" [saveUrl]="saveURL" [customFileDetails]="customFileDetails" [removeUrl]="removeURL"></ej-uploadbox>
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
  saveURL: string;
  removeURL: string;
  customFileDetails: Object;
  constructor() {
  this.saveURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Save';
  this.removeURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Remove';
  this.customFileDetails={ title:true, name:true, size:true, status:true, action:true};
  }
}


{% endhighlight %}









### customFileDetails.action `boolean`
{:#members:customfiledetails-action}








Enables the file upload interactions like remove/cancel in File details of the dialog popup.













### customFileDetails.name `boolean`
{:#members:customfiledetails-name}








Enables the name in the File details of the dialog popup.











### customFileDetails.size `boolean`
{:#members:customfiledetails-size}








Enables or disables the File size details of the dialog popup.

N>  Details of the File Size is available from IE10+ browser version.













### customFileDetails.status `boolean`
{:#members:customfiledetails-status}








Enables or disables the file uploading status visibility in the dialog file details content.












### customFileDetails.title `boolean`
{:#members:customfiledetails-title}








Enables the title in File details for the dialog popup.










### dialogAction `object`
{:#members:dialogaction}








Specifies the actions for dialog popup while initialization.




#### Default Value







* { modal:false, closeOnComplete:false, content:null, drag:true}








#### Example

{% highlight html %}

<div id="upload_controls" style="margin-left: 35%;">
<div>Select a file to upload</div>
<div style="width:100px;height:35px;">
    <ej-uploadbox id="uploadDefault" [dialogAction]="dialogAction" [saveUrl]="saveURL" [removeUrl]="removeURL"></ej-uploadbox>
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
  saveURL: string;
  removeURL: string;
  dialogAction: any;
  constructor() {
  this.saveURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Save';
  this.removeURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Remove';
  this. dialogAction= { modal:false, closeOnComplete:true,resize: true, drag:true, content:"#uploadDefault"};
  }
}


{% endhighlight %}









### dialogAction.closeOnComplete `boolean`
{:#members:dialogaction-closeoncomplete}








Once uploaded successfully, the dialog popup closes immediately.












### dialogAction.content `string`
{:#members:dialogaction-content}








Sets the content container option to the Uploadbox dialog popup.











### dialogAction.drag `boolean`
{:#members:dialogaction-drag}








Enables the drag option to the dialog popup.












### dialogAction.modal `boolean`
{:#members:dialogaction-modal}








Enables or disables the Uploadbox dialog’s modal property to the dialog popup.


N> dialogAction.modal property does not work in synchronous file upload.












### dialogPosition `object`
{:#members:dialogposition}








Displays the Uploadbox dialog at the given X and Y positions. X: Dialog sets the left position value. Y: Dialog sets the top position value.




#### Default Value







* null








#### Example

{% highlight html %}

<div id="upload_controls" style="margin-left: 35%;">
<div>Select a file to upload</div>
<div style="width:100px;height:35px;">
    <ej-uploadbox id="uploadDefault" [dialogPosition]="dialogPosition" [saveUrl]="saveURL" [removeUrl]="removeURL"></ej-uploadbox>
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
  saveURL: string;
  removeURL: string;
  dialogPosition: any;
  constructor() {
  this.saveURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Save';
  this.removeURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Remove';
  this.dialogPosition= { X: 300, Y: 10 };
  }
}


{% endhighlight %}










### dialogText `object`
{:#members:dialogtext}








Property for applying the text to the Dialog title and content headers.




#### Default Value







* { title: "Upload Box", name: "Name", size: "Size", status: "Status"}








#### Example

{% highlight html %}

<div id="upload_controls" style="margin-left: 35%;">
<div>Select a file to upload</div>
<div style="width:100px;height:35px;">
    <ej-uploadbox id="uploadDefault" [dialogText]="dialogText" [saveUrl]="saveURL" [removeUrl]="removeURL"></ej-uploadbox>
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
  saveURL: string;
  removeURL: string;
  dialogText: any;
  constructor() {
  this.saveURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Save';
  this.removeURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Remove';
  this.dialogText = {title:"Upload File List",name:"File Name",size:"File Size",status:"File Status" };
  }
}


{% endhighlight %}










### dialogText.name `string`
{:#members:dialogtext-name}








Sets the uploaded file’s Name (header text) to the Dialog popup.












### dialogText.size `string`
{:#members:dialogtext-size}








Sets the upload file Size (header text) to the dialog popup.












### dialogText.status `string`
{:#members:dialogtext-status}








Sets the upload file Status (header text) to the dialog popup.











### dialogText.title `string`
{:#members:dialogtext-title}








Sets the title text of the dialog popup.












### dropAreaText `string`
{:#members:dragareatext}








The dropAreaText is displayed when the drag and drop support is enabled in the Uploadbox control.




#### Default Value







* "Drop files or click to upload"








#### Example

{% highlight html %}

<div id="upload_controls" style="margin-left: 35%;">
<div>Select a file to upload</div>
<div style="width:100px;height:35px;">
    <ej-uploadbox id="uploadDefault" [allowDragAndDrop]=true  dropAreaText="Drop files or click to upload" [saveUrl]="saveURL" [removeUrl]="removeURL"></ej-uploadbox>
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
  saveURL: string;
  removeURL: string;
  
  constructor() {
  this.saveURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Save';
  this.removeURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Remove';
  
  }
}


{% endhighlight %}









### dropAreaHeight `number`  `string`
{:#members:dropareaheight}








Specifies the dropAreaHeight when the drag and drop support is enabled in the Uploadbox control.




#### Default Value







* "100%"








#### Example

{% highlight html %}

<div id="upload_controls" style="margin-left: 35%;">
<div>Select a file to upload</div>
<div style="width:100px;height:35px;">
    <ej-uploadbox id="uploadDefault" [allowDragAndDrop]=true dropAreaHeight="100%" dropAreaText="Drop files or click to upload" [saveUrl]="saveURL" [removeUrl]="removeURL"></ej-uploadbox>
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
  saveURL: string;
  removeURL: string;
  
  constructor() {
  this.saveURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Save';
  this.removeURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Remove';
  
  }
}


{% endhighlight %}










### dropAreaWidth `number|string`
{:#members:dropareawidth}








Specifies the dropAreaWidth when the drag and drop support is enabled in the Uploadbox control.




#### Default Value







* "100%"








#### Example

{% highlight html %}

<div id="upload_controls" style="margin-left: 35%;">
<div>Select a file to upload</div>
<div style="width:100px;height:35px;">
    <ej-uploadbox id="uploadDefault" [allowDragAndDrop]=true dropAreaWidth="100%" dropAreaText="Drop files or click to upload" [saveUrl]="saveURL" [removeUrl]="removeURL"></ej-uploadbox>
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
  saveURL: string;
  removeURL: string;
  
  constructor() {
  this.saveURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Save';
  this.removeURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Remove';
  
  }
}


{% endhighlight %}










### enabled `boolean`
{:#members:enabled}







Based on the property value, Uploadbox is enabled or disabled.




#### Default Value







* true








#### Example

{% highlight html %}

<div id="upload_controls" style="margin-left: 35%;">
<div>Select a file to upload</div>
<div style="width:100px;height:35px;">
    <ej-uploadbox id="uploadDefault" [enabled]=true [saveUrl]="saveURL" [removeUrl]="removeURL"></ej-uploadbox>
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
  saveURL: string;
  removeURL: string;
  
  constructor() {
  this.saveURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Save';
  this.removeURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Remove';
  
  }
}


{% endhighlight %}










### enableRTL `boolean`
{:#members:enablertl}








Sets the right-to-left direction property for the Uploadbox control.




#### Default Value







* false








#### Example

{% highlight html %}

<div id="upload_controls" style="margin-left: 35%;">
<div>Select a file to upload</div>
<div style="width:100px;height:35px;">
    <ej-uploadbox id="uploadDefault" [enableRTL]=true  [saveUrl]="saveURL" [removeUrl]="removeURL"></ej-uploadbox>
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
  saveURL: string;
  removeURL: string;
  
  constructor() {
  this.saveURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Save';
  this.removeURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Remove';
  
  }
}


{% endhighlight %}









### extensionsAllow `string`
{:#members:extensionsallow}








Only the files with the specified extension is allowed to upload. This is mentioned in the string format.




#### Default Value







* ""








#### Example

{% highlight html %}

<div id="upload_controls" style="margin-left: 35%;">
<div>Select a file to upload</div>
<div style="width:100px;height:35px;">
    <ej-uploadbox id="uploadDefault" extensionsAllow=".zip" [saveUrl]="saveURL" [removeUrl]="removeURL"></ej-uploadbox>
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
  saveURL: string;
  removeURL: string;
  
  constructor() {
  this.saveURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Save';
  this.removeURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Remove';
  
  }
}


{% endhighlight %}











### extensionsDeny `string`
{:#members:extensionsdeny}








Only the files with the specified extension is denied for upload. This is mentioned in the string format.




#### Default Value







* ""








#### Example

{% highlight html %}

<div id="upload_controls" style="margin-left: 35%;">
<div>Select a file to upload</div>
<div style="width:100px;height:35px;">
    <ej-uploadbox id="uploadDefault" extensionsDeny=".zip" [saveUrl]="saveURL" [removeUrl]="removeURL"></ej-uploadbox>
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
  saveURL: string;
  removeURL: string;
  
  constructor() {
  this.saveURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Save';
  this.removeURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Remove';
  
  }
}


{% endhighlight %}











### fileSize `number`
{:#members:filesize}








Sets the maximum size limit for uploading the file. This is mentioned in the number format.

N> fileSize represents the size of the individual file.





#### Default Value







* 31457280








#### Example

{% highlight html %}

<div id="upload_controls" style="margin-left: 35%;">
<div>Select a file to upload</div>
<div style="width:100px;height:35px;">
    <ej-uploadbox id="uploadDefault" [fileSize]="fileSize" [saveUrl]="saveURL" [removeUrl]="removeURL"></ej-uploadbox>
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
  saveURL: string;
  removeURL: string;
  fileSize: number;
  constructor() {
  this.saveURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Save';
  this.removeURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Remove';
  this.fileSize = 31457280;
  }
}


{% endhighlight %}










### height `string`
{:#members:height}








Sets the height of the browse button.




#### Default Value







* 35px








#### Example

{% highlight html %}

<div id="upload_controls" style="margin-left: 35%;">
<div>Select a file to upload</div>
<div style="width:100px;height:35px;">
    <ej-uploadbox id="uploadDefault" height="40px" [saveUrl]="saveURL" [removeUrl]="removeURL"></ej-uploadbox>
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
  saveURL: string;
  removeURL: string;
  
  constructor() {
  this.saveURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Save';
  this.removeURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Remove';
  
  }
}


{% endhighlight %}







### htmlAttributes `object`

{:#members:htmlattributes}
 
Specifies the list of HTML attributes to be added to uploadbox control.
 
#### Default Value
 
* {}
 
#### Example 

{% highlight html %}

<div id="upload_controls" style="margin-left: 35%;">
<div>Select a file to upload</div>
<div style="width:100px;height:35px;">
    <ej-uploadbox id="uploadDefault" [htmlAttributes]="attributes" [saveUrl]="saveURL" [removeUrl]="removeURL"></ej-uploadbox>
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
  saveURL: string;
  removeURL: string;
  attributes: Object;
  constructor() {
  this.saveURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Save';
  this.removeURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Remove';
  this.attributes={"aria-label":"uploadbox"};
  }
}


{% endhighlight %}






### locale `string`
{:#members:locale}








Configures the culture data and sets the culture to the Uploadbox.




#### Default Value







* "en-US"








#### Example

{% highlight html %}

<div id="upload_controls" style="margin-left: 35%;">
<div>Select a file to upload</div>
<div style="width:100px;height:35px;">
    <ej-uploadbox id="uploadDefault" locale="nl-BE" [saveUrl]="saveURL" [removeUrl]="removeURL"></ej-uploadbox>
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
  saveURL: string;
  removeURL: string;
  
  constructor() {
  this.saveURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Save';
  this.removeURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Remove';
  
  }
}
ej.Uploadbox.Locale["nl-BE"] = {
        buttonText: {
            upload: "uploaden",
            browse: "Blader",
            cancel: "Annuleer",
            close: "dicht"
        },
        dialogText: {
            title: "Upload Box",
            name: "naam",
            size: "grootte",
            status: "toestand"
        },
        dropAreaText: "Drop bestanden of klik te uploaden ",
        filedetail: "Het geselecteerde bestand is te groot . Selecteer een bestand in de geldige grootte.",
        denyError: "Bestanden met #Extension extensies zijn niet toegestaan.",
        allowError: "Alleen bestanden met #Extension extensies zijn toegestaan.",
        cancelToolTip: "Annuleer",
        removeToolTip: "verwijderen",
        retryToolTip: "opnieuw proberen",
        completedToolTip: "voltooid",
        failedToolTip: "gefaald",
        closeToolTip: "dicht"
    }; 

{% endhighlight %}










### multipleFilesSelection `boolean`
{:#members:multiplefilesselection}








Enables multiple file selection for upload.




#### Default Value







* true








#### Example

{% highlight html %}

<div id="upload_controls" style="margin-left: 35%;">
<div>Select a file to upload</div>
<div style="width:100px;height:35px;">
    <ej-uploadbox id="uploadDefault" [multipleFilesSelection]=true [saveUrl]="saveURL" [removeUrl]="removeURL"></ej-uploadbox>
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
  saveURL: string;
  removeURL: string;
  
  constructor() {
  this.saveURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Save';
  this.removeURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Remove';
  
  }
}


{% endhighlight %}











### pushFile `object`
{:#members:pushfile}








You can push the file to the Uploadbox in the client-side of the XHR supported browsers alone.




#### Default Value







* null








#### Example

{% highlight html %}

<div id="upload_controls" style="margin-left: 35%;">
<div>Select a file to upload</div>
<div style="width:100px;height:35px;">
    <ej-uploadbox id="uploadDefault" [pushFile]="pushFile" [saveUrl]="saveURL" [removeUrl]="removeURL"></ej-uploadbox>
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
  saveURL: string;
  removeURL: string;
  pushFile: any;
  constructor() {
  this.saveURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Save';
  this.removeURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Remove';
  this.pushFile= files;
  }
}


{% endhighlight %}











### removeUrl `string`
{:#members:removeurl}








Specifies the remove action to be performed after the file uploading is completed. Here, mention the server address for removal.




#### Default Value







* ""








#### Example

{% highlight html %}

<div id="upload_controls" style="margin-left: 35%;">
<div>Select a file to upload</div>
<div style="width:100px;height:35px;">
    <ej-uploadbox id="uploadDefault" [saveUrl]="saveURL" [removeUrl]="removeURL"></ej-uploadbox>
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
  saveURL: string;
  removeURL: string;
  
  constructor() {
  this.saveURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Save';
  this.removeURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Remove';
  
  }
}


{% endhighlight %}












### saveUrl `string`
{:#members:saveurl}








Specifies the save action to be performed after the file is pushed for uploading. Here, mention the server address to be saved. 




#### Default Value







* ""








#### Example

{% highlight html %}

<div id="upload_controls" style="margin-left: 35%;">
<div>Select a file to upload</div>
<div style="width:100px;height:35px;">
    <ej-uploadbox id="uploadDefault" [saveUrl]="saveURL" [removeUrl]="removeURL"></ej-uploadbox>
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
  saveURL: string;
  removeURL: string;
  
  constructor() {
  this.saveURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Save';
  this.removeURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Remove';
  
  }
}


{% endhighlight %}












### showBrowseButton `boolean`
{:#members:showbrowsebutton}








Enables the browse button support to the Uploadbox control.




#### Default Value







* true








#### Example

{% highlight html %}

<div id="upload_controls" style="margin-left: 35%;">
<div>Select a file to upload</div>
<div style="width:100px;height:35px;">
    <ej-uploadbox id="uploadDefault" [showBrowseButton]=true [saveUrl]="saveURL" [removeUrl]="removeURL"></ej-uploadbox>
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
  saveURL: string;
  removeURL: string;
  
  constructor() {
  this.saveURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Save';
  this.removeURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Remove';
  
  }
}


{% endhighlight %}











### showFileDetails `boolean`
{:#members:showfiledetails}








Specifies the file details to be displayed when selected for uploading. This can be done when the showFileDetails is set to true.



#### Default Value







* true








#### Example

{% highlight html %}

<div id="upload_controls" style="margin-left: 35%;">
<div>Select a file to upload</div>
<div style="width:100px;height:35px;">
    <ej-uploadbox id="uploadDefault" [showFileDetails]=true [saveUrl]="saveURL" [removeUrl]="removeURL"></ej-uploadbox>
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
  saveURL: string;
  removeURL: string;
  
  constructor() {
  this.saveURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Save';
  this.removeURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Remove';
  
  }
}


{% endhighlight %}







### showRoundedCorner `boolean`
{:#members:showroundedcorner} 

Specifies the file details to be displayed when selected for uploading. This can be done when the showFileDetails is set to true.
 
#### Default Value 
 
* true
 
#### Example

{% highlight html %}

<div id="upload_controls" style="margin-left: 35%;">
<div>Select a file to upload</div>
<div style="width:100px;height:35px;">
    <ej-uploadbox id="uploadDefault" [enabled]=true [saveUrl]="saveURL" [removeUrl]="removeURL"></ej-uploadbox>
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
  saveURL: string;
  removeURL: string;
  
  constructor() {
  this.saveURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Save';
  this.removeURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Remove';
  
  }
}


{% endhighlight %}



 


### uploadName `string`
{:#members:uploadname}








Sets the name for the Uploadbox control. This API helps to Map the action in code behind to retrieve the files.





#### Default Value







* ""








#### Example

{% highlight html %}

<div id="upload_controls" style="margin-left: 35%;">
<div>Select a file to upload</div>
<div style="width:100px;height:35px;">
    <ej-uploadbox id="uploadDefault" uploadName="Uploadbox" [saveUrl]="saveURL" [removeUrl]="removeURL"></ej-uploadbox>
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
  saveURL: string;
  removeURL: string;
  
  constructor() {
  this.saveURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Save';
  this.removeURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Remove';
  
  }
}


{% endhighlight %}











### width `string`
{:#members:width}








Sets the width of the browse button.




#### Default Value







* 100px








#### Example

{% highlight html %}

<div id="upload_controls" style="margin-left: 35%;">
<div>Select a file to upload</div>
<div style="width:100px;height:35px;">
    <ej-uploadbox id="uploadDefault" uploadName="Uploadbox" [saveUrl]="saveURL" [removeUrl]="removeURL"></ej-uploadbox>
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
  saveURL: string;
  removeURL: string;
  
  constructor() {
  this.saveURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Save';
  this.removeURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Remove';
  
  }
}


{% endhighlight %}










## Methods








### destroy()
{:#methods:destroy}








The destroy method destroys the control and brings the control to a pre-init state. All the events of the Upload control is bound by using this._on unbinds automatically.  





#### Example

{% highlight html %}

<div id="upload_controls" style="margin-left: 35%;">
<div>Select a file to upload</div>
<div style="width:100px;height:35px;">
    <ej-uploadbox id="uploadDefault" [enabled]=true [saveUrl]="saveURL" [removeUrl]="removeURL"></ej-uploadbox>
</div>
</div>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Destroy</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  saveURL: string;
  removeURL: string;
  
  constructor() {
  this.saveURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Save';
  this.removeURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Remove';
  
  }
  OnClick(){
      var obj = $("#uploadDefault").data("ejUploadbox");

  obj.destroy();
  }
}


{% endhighlight %}

{% highlight html %}

<div id="upload_controls" style="margin-left: 35%;">
<div>Select a file to upload</div>
<div style="width:100px;height:35px;">
    <ej-uploadbox id="uploadDefault" [enabled]=true [saveUrl]="saveURL" [removeUrl]="removeURL"></ej-uploadbox>
</div>
</div>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Destroy</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  saveURL: string;
  removeURL: string;
  
  constructor() {
  this.saveURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Save';
  this.removeURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Remove';
  
  }
  OnClick(){


$("#uploadDefault").ejUploadbox("destroy");
  }
}


{% endhighlight %}











### disable()
{:#methods:disable}








Disables the Uploadbox control





#### Example

{% highlight html %}

<div id="upload_controls" style="margin-left: 35%;">
<div>Select a file to upload</div>
<div style="width:100px;height:35px;">
    <ej-uploadbox id="uploadDefault" [enabled]=true [saveUrl]="saveURL" [removeUrl]="removeURL"></ej-uploadbox>
</div>
</div>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Disable</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  saveURL: string;
  removeURL: string;
  
  constructor() {
  this.saveURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Save';
  this.removeURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Remove';
  
  }
  OnClick(){
      var obj = $("#uploadDefault").data("ejUploadBox");

  obj.disable();


$("#uploadDefault").ejUploadBox("disable");
  }
}


{% endhighlight %}

{% highlight html %}

<div id="upload_controls" style="margin-left: 35%;">
<div>Select a file to upload</div>
<div style="width:100px;height:35px;">
    <ej-uploadbox id="uploadDefault" [enabled]=true [saveUrl]="saveURL" [removeUrl]="removeURL"></ej-uploadbox>
</div>
</div>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Disable</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  saveURL: string;
  removeURL: string;
  
  constructor() {
  this.saveURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Save';
  this.removeURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Remove';
  
  }
  OnClick(){


$("#uploadDefault").ejUploadBox("disable");
  }
}


{% endhighlight %}










### enable()
{:#methods:enable}








Enables the Uploadbox control





#### Example

{% highlight html %}

<div id="upload_controls" style="margin-left: 35%;">
<div>Select a file to upload</div>
<div style="width:100px;height:35px;">
    <ej-uploadbox id="uploadDefault" [enabled]=true [saveUrl]="saveURL" [removeUrl]="removeURL"></ej-uploadbox>
</div>
</div>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Enable</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  saveURL: string;
  removeURL: string;
  
  constructor() {
  this.saveURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Save';
  this.removeURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Remove';
  
  }
  OnClick(){
      var obj = $("#uploadDefault").data("ejUploadbox");

  obj.enable();



  }
}


{% endhighlight %}

{% highlight html %}

<div id="upload_controls" style="margin-left: 35%;">
<div>Select a file to upload</div>
<div style="width:100px;height:35px;">
    <ej-uploadbox id="uploadDefault" [enabled]=true [saveUrl]="saveURL" [removeUrl]="removeURL"></ej-uploadbox>
</div>
</div>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Enable</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  saveURL: string;
  removeURL: string;
  
  constructor() {
  this.saveURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Save';
  this.removeURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Remove';
  
  }
  OnClick(){


$("#uploadDefault").ejUploadbox("enable");
  }
}


{% endhighlight %}




### refresh()
{:#methods:refresh}

Refresh the Uploadbox control
 
#### Example

{% highlight html %}

<div id="upload_controls" style="margin-left: 35%;">
<div>Select a file to upload</div>
<div style="width:100px;height:35px;">
    <ej-uploadbox id="uploadDefault" [enabled]=true [saveUrl]="saveURL" [removeUrl]="removeURL"></ej-uploadbox>
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
  saveURL: string;
  removeURL: string;
  
  constructor() {
  this.saveURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Save';
  this.removeURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Remove';
  
  }
  OnClick(){
      var obj = $("#uploadDefault").data("ejUploadbox");

  obj.refresh();



  }
}


{% endhighlight %}

{% highlight html %}

<div id="upload_controls" style="margin-left: 35%;">
<div>Select a file to upload</div>
<div style="width:100px;height:35px;">
    <ej-uploadbox id="uploadDefault" [enabled]=true [saveUrl]="saveURL" [removeUrl]="removeURL"></ej-uploadbox>
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
  saveURL: string;
  removeURL: string;
  
  constructor() {
  this.saveURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Save';
  this.removeURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Remove';
  
  }
  OnClick(){


$("#uploadDefault").ejUploadbox("refresh");
  }
}


{% endhighlight %}







### upload()
{:#methods:upload}

Upload the selected files.
 
#### Example

{% highlight html %}

<div id="upload_controls" style="margin-left: 35%;">
<div>Select a file to upload</div>
<div style="width:100px;height:35px;">
    <ej-uploadbox id="uploadDefault" [enabled]=true [showFileDetails]=false [saveUrl]="saveURL" [removeUrl]="removeURL"></ej-uploadbox>
</div>
</div>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Upload</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  saveURL: string;
  removeURL: string;
  
  constructor() {
  this.saveURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Save';
  this.removeURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Remove';
  
  }
  OnClick(){
      var obj = $("#uploadDefault").data("ejUploadbox");

  obj.upload();



  }
}


{% endhighlight %}

{% highlight html %}

<div id="upload_controls" style="margin-left: 35%;">
<div>Select a file to upload</div>
<div style="width:100px;height:35px;">
    <ej-uploadbox id="uploadDefault" [enabled]=true [showFileDetails]=false [saveUrl]="saveURL" [removeUrl]="removeURL"></ej-uploadbox>
</div>
</div>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Upload</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  saveURL: string;
  removeURL: string;
  
  constructor() {
  this.saveURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Save';
  this.removeURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Remove';
  
  }
  OnClick(){


$("#uploadDefault").ejUploadbox("upload");
  }
}


{% endhighlight %}






## Events







### beforeSend
{:#events:beforesend}
 
Fires when the upload progress beforeSend.
 
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
<td class="name">files</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Selected FileList Object.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the Uploadbox model</td>
</tr>
<tr>
<td class="name">xhr</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">XHR-AJAX Object for reference.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<div id="upload_controls" style="margin-left: 35%;">
<div>Select a file to upload</div>
<div style="width:100px;height:35px;">
    <ej-uploadbox id="uploadDefault" [enabled]=true [saveUrl]="saveURL" [removeUrl]="removeURL" (beforeSend)="beforeSend($create)"></ej-uploadbox>
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
  saveURL: string;
  removeURL: string;
  
  constructor() {
  this.saveURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Save';
  this.removeURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Remove';
  
  }
  beforeSend(args){
     
  }
}


{% endhighlight %}




### begin
{:#events:begin}








Fires when the upload progress begins.


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
<td class="type"><span class="param-type">object</span></td>
<td class="description">To pass additional information to the server.</td>
</tr>
<tr>
<td class="name">files</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Selected FileList Object.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the Uploadbox model</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<div id="upload_controls" style="margin-left: 35%;">
<div>Select a file to upload</div>
<div style="width:100px;height:35px;">
    <ej-uploadbox id="uploadDefault" [enabled]=true [saveUrl]="saveURL" [removeUrl]="removeURL" (begin)="begin($create)"></ej-uploadbox>
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
  saveURL: string;
  removeURL: string;
  
  constructor() {
  this.saveURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Save';
  this.removeURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Remove';
  
  }
  begin(args){
     
  }
}


{% endhighlight %}









### cancel
{:#events:cancel}








Fires when the upload progress is cancelled.

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
<td class="name">fileStatus</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Canceled FileList Object.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the Uploadbox model</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<div id="upload_controls" style="margin-left: 35%;">
<div>Select a file to upload</div>
<div style="width:100px;height:35px;">
    <ej-uploadbox id="uploadDefault" [enabled]=true [saveUrl]="saveURL" [removeUrl]="removeURL" (cancel)="cancel($create)"></ej-uploadbox>
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
  saveURL: string;
  removeURL: string;
  
  constructor() {
  this.saveURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Save';
  this.removeURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Remove';
  
  }
  cancel(args){
     
  }
}


{% endhighlight %}









### complete
{:#events:complete}








Fires when the file upload progress is completed.

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
<td class="name">e</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">AJAX event argument for reference.</td>
</tr>
<tr>
<td class="name">files</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Uploaded file list.</td>
</tr>
<tr>
<td class="name">responseText</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">response from the server.</td>
</tr>
<tr>
<td class="name">xhr</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">XHR-AJAX Object for reference.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the Uploadbox model</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>



#### Example

{% highlight html %}

<div id="upload_controls" style="margin-left: 35%;">
<div>Select a file to upload</div>
<div style="width:100px;height:35px;">
    <ej-uploadbox id="uploadDefault" [enabled]=true [saveUrl]="saveURL" [removeUrl]="removeURL" (complete)="complete($create)"></ej-uploadbox>
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
  saveURL: string;
  removeURL: string;
  
  constructor() {
  this.saveURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Save';
  this.removeURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Remove';
  
  }
  complete(args){
     
  }
}


{% endhighlight %}








### success
{:#events:success}








Fires when the file upload progress is succeeded.

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
<td class="name">responseText</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">response from the server.</td>
</tr>
<tr>
<td class="name">e</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">AJAX event argument for reference.</td>
</tr>
<tr>
<td class="name">success</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">successfully uploaded files list.</td>
</tr>
<tr>
<td class="name">files</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Uploaded file list.</td>
</tr>
<tr>
<td class="name">xhr</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">XHR-AJAX Object for reference.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the Uploadbox model</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<div id="upload_controls" style="margin-left: 35%;">
<div>Select a file to upload</div>
<div style="width:100px;height:35px;">
    <ej-uploadbox id="uploadDefault" [enabled]=true [saveUrl]="saveURL" [removeUrl]="removeURL" (success)="success($create)"></ej-uploadbox>
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
  saveURL: string;
  removeURL: string;
  
  constructor() {
  this.saveURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Save';
  this.removeURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Remove';
  
  }
  success(args){
     
  }
}


{% endhighlight %}










### create
{:#events:create}








Fires when the Uploadbox control is created.

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
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the Uploadbox model</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>



#### Example

{% highlight html %}

<div id="upload_controls" style="margin-left: 35%;">
<div>Select a file to upload</div>
<div style="width:100px;height:35px;">
    <ej-uploadbox id="uploadDefault" [enabled]=true [saveUrl]="saveURL" [removeUrl]="removeURL" (create)="create($create)"></ej-uploadbox>
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
  saveURL: string;
  removeURL: string;
  
  constructor() {
  this.saveURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Save';
  this.removeURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Remove';
  
  }
  create(args){
     
  }
}


{% endhighlight %}








### destroy
{:#events:destroy}








Fires when the Uploadbox control is destroyed.

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
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the Uploadbox model</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>




#### Example

{% highlight html %}

<div id="upload_controls" style="margin-left: 35%;">
<div>Select a file to upload</div>
<div style="width:100px;height:35px;">
    <ej-uploadbox id="uploadDefault" [enabled]=true [saveUrl]="saveURL" [removeUrl]="removeURL" (destroy)="destroy($create)"></ej-uploadbox>
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
  saveURL: string;
  removeURL: string;
  
  constructor() {
  this.saveURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Save';
  this.removeURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Remove';
  
  }
  destroy(args){
     
  }
}


{% endhighlight %}









### error
{:#events:error}








Fires when the Upload process ends in Error.

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
<td class="name">error</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">details about the error information.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
<tr>
<td class="name">action</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">error event action details.</td>
</tr>
<tr>
<td class="name">files</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the file details of the file uploaded</td>
</tr>
</tbody>
</table>




#### Example

{% highlight html %}

<div id="upload_controls" style="margin-left: 35%;">
<div>Select a file to upload</div>
<div style="width:100px;height:35px;">
    <ej-uploadbox id="uploadDefault" [enabled]=true [saveUrl]="saveURL" [removeUrl]="removeURL" (error)="error($create)"></ej-uploadbox>
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
  saveURL: string;
  removeURL: string;
  
  constructor() {
  this.saveURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Save';
  this.removeURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Remove';
  
  }
  error(args){
     
  }
}


{% endhighlight %}








### fileSelect
{:#events:fileselect}








Fires when the file is selected for upload successfully.

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
<td class="name">files</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns Selected FileList objects</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the Uploadbox model</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<div id="upload_controls" style="margin-left: 35%;">
<div>Select a file to upload</div>
<div style="width:100px;height:35px;">
    <ej-uploadbox id="uploadDefault" [enabled]=true [saveUrl]="saveURL" [removeUrl]="removeURL" (fileSelect)="fileSelect($create)"></ej-uploadbox>
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
  saveURL: string;
  removeURL: string;
  
  constructor() {
  this.saveURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Save';
  this.removeURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Remove';
  
  }
  fileSelect(args){
     
  }
}


{% endhighlight %}




### inProgress
{:#events:inprogress}
  
Fires when the file is uploading.

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
<td class="name">e</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">AJAX event argument for reference.</td>
</tr>
<tr>
<td class="name">files</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns Selected FileList objects</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the Uploadbox model</td>
</tr>
<tr>
<td class="name">percentage</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the current progress percentage.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>
 
#### Example

{% highlight html %}

<div id="upload_controls" style="margin-left: 35%;">
<div>Select a file to upload</div>
<div style="width:100px;height:35px;">
    <ej-uploadbox id="uploadDefault" [enabled]=true [saveUrl]="saveURL" [removeUrl]="removeURL" (inProgress)="inProgress($create)"></ej-uploadbox>
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
  saveURL: string;
  removeURL: string;
  
  constructor() {
  this.saveURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Save';
  this.removeURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Remove';
  
  }
  inProgress(args){
     
  }
}


{% endhighlight %}







### remove
{:#events:remove}








Fires when the uploaded file is removed successfully.

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
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the Uploadbox model</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
<tr>
<td class="name">fileStatus</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the file details of the file object</td>
</tr>
</tbody>
</table>




#### Example

{% highlight html %}

<div id="upload_controls" style="margin-left: 35%;">
<div>Select a file to upload</div>
<div style="width:100px;height:35px;">
    <ej-uploadbox id="uploadDefault" [enabled]=true [saveUrl]="saveURL" [removeUrl]="removeURL" (remove)="remove($create)"></ej-uploadbox>
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
  saveURL: string;
  removeURL: string;
  
  constructor() {
  this.saveURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Save';
  this.removeURL = 'http://js.syncfusion.com/ejServices/api/uploadbox/Remove';
  
  }
  remove(args){
     
  }
}


{% endhighlight %}


 
