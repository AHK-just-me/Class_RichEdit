# Class_RichEdit #

### AHK RichEdit Control ###

AHK class providing support for **RICHEDIT50W** controls in AHK GUIs.

In the *Sources* folder you'll find three scripts and one RTF test file:

1. **Class_RichEdit.ahk** - contains the class definition.
2. **Class_RichEditDlgs.ahk** - contains common dialogs definitions used in the sample script. It is not needed to use the class, you might simply ignore it.
3. **RichEdit_sample.ahk** - is a sample script showing how to use the RichEdit control.
4. **Test.rtf** - RTF test file.

### How to start ###

At first, look at the sample script, please. It is (clearly) showing how to use the class to create and use RichEdit controls. It contains calls of the most important methods provided by the class. 

To add a RichEdit control to your GUI just create a *new* instance of the *RichEdit* class, passing the GUI name and the control's options, if needed. The options may contain the control's position and dimension like used with `Gui, Add` as well as an optional *gLabel*. The constructor will add the control as a *Custom*, *ClassRICHEDIT50W*. If you don't pass options for positioning and sizing, the GUI respectively the control's defaults will be used. The current GUI font will be set as default. Also, appropriate styles are set automatically, so you must not pass style options.

After the control is created, you may set general options as defaults for the control calling the appropriate methods. Now preparation is finished.

Some of the RichEdit's functionality is working out of the box by shortcuts as shown on [MSDN](http://msdn.microsoft.com/en-us/library/bb787873%28v=vs.85%29.aspx#rich_edit_shortcut_keys "http://msdn.microsoft.com/en-us/library/bb787873(v=vs.85).aspx#rich_edit_shortcut_keys"). But not all of them are working as documented. Aside from that, some of them cannot be used on non-english keyboards. So you'll quickly realise, that RichEdit's are easy to create, but hard to use.

### And now the ball's in your court! ###
