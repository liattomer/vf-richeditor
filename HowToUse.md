# How To Use #

## Introduction ##

Microsoft-word like editing of text within [Salesforce.com](http://www.salesforce.com) and the [Force.com platform](http://developer.force.com/gettingstarted). It is based on the open-source [fckEditor](http://www.fckeditor.net/) created by Frederico Caldeira Knabben. When implemented within a Visualforce page, the end user will have the ability to see and edit text including fonts, colors, alignment, bullets, links, images, and more.

## Installing the Component ##

After downloading richeditor.zip, unzip the contents to a temporary folder. Inside you will find four files described below:

The first file "fckeditor.zip" contains the implementation of the editor. You must upload this to Salesforce as a static resource. Please name the static resource "fckEditor".

The second file is "richeditor.component". This is just a text file contained the code for the Visualforce component. Copy and past the contents of this file into a new Visualforce component called "RichEditor". Alternatively, you can drag and drop this file along with "richeditor.component-meta.xml" onto the "components" folder of a Force.com project inside the Force.com IDE to install it.

The last file "how-to.txt" contains these instructions.

## Using the Component ##

To use the Rich Editor component within a Visualforce page, simply declare the tag like while assigning a value property that is a text field.

```
<c:RichEditor value="{!account.Description}"/>
```

Other than the value attribute (required) there are two additional optional attributes:

width - the width of the editor
height - the height of the editor

The editor itself is highly configurable. Most of the configuration options can be changed via a file called "customconfig.js" inside the "fckeditor.zip" file. For more information on what options exist, consult the [fckeditor developer's guide](http://docs.fckeditor.net/FCKeditor_2.x/Developers_Guide).