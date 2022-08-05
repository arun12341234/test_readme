# GUI Operations

***This plugin that works across Windows, MacOS X and Linux which provides the ability to simulate mouse cursor moves and Some Message box..***



## Numerical Basic Operations
Item | Value
---|:---:
Icon | ![GUI Operations](icon.png) 
Display Name | **GUI Operations**

## Name of the author (Contact info of the author)

Pavan K
* [email](mailto:pvnpavank@argos-labs.com) 
 
## Version Control 
* [4.503.1000](setup.yaml)
* Release Date: `May 03, 2022`

## Input (Required)
Display Name | Selection | Default Value | Description| Input| Output
---|---|---|---|---|---
Operation |Screen Size |Screen Size |  Get the size of the primary monitor or display.|*None*|(1366,766)| 
 &nbsp;|Alert|&nbsp;|Displays a simple message box with text and a single OK button. Returns the text of the button clicked on. | message='Sample Message' |![Alert Box](README_alert.jpg)|
&nbsp;|Confirm Prompt |&nbsp;|Displays a message box with OK and Cancel buttons. Number and text of buttons can be customized. Returns the text of the button clicked on. | title='Test Title' </br>message='Sample Message'|![Confirm Box](README_confirm.jpg)|  
&nbsp;|Vertical Scroll |&nbsp;|The mouse scroll wheel can be simulated by calling the scroll() function and passing an integer number of “clicks” to scroll. The amount of scrolling in a “click” varies between platforms. Optionally, integers can be passed for the the x and y keyword arguments to move the mouse cursor before performing the scroll. | lines= 50 </br>lines= -50|positive input  # scroll up 50 "clicks" and negative input  #scroll down 50 "clicks"| 
&nbsp;|Horizontal Scroll |&nbsp;|On only OS X and Linux platforms, Horizontal scroll will works and passing an integer number of “clicks” to scroll. The amount of scrolling in a “click” varies between platforms. Optionally, integers can be passed for the the x and y keyword arguments to move the mouse cursor before performing the scroll. | lines= 50 </br>lines= -50|positive input  # scroll right 50 "clicks and negative input  #scroll left 50 "clicks|  
## Return Value

### Normal Case
Description of output result

## Return Code
Code | Meaning
---|---
0 | Success
99 | Exceptional case

##Output Format
You may choose one of 3 output formats below,

<ul>
  <li>String (default)</li>
  <li>CSV</li>
  <li>File</li>
</ul>  

 
