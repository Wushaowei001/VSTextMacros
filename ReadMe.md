What is it?
===============================

An extension for Visual Studio 2012/2013 that brings back support for macros in text/code editors. These macros can be used to automate repetitive text editing tasks.

You may have used such macros in previous versions of Visual Studio. Indeed, macros used to be supported and [removed][5] in Visual Studio 2010.

Although macros used to be very sophisticated at the time, letting you control almost any feature of Visual Studio, this extension only aims at supporting the text editing part of macros.

And if you have not used Visual Studio macros before, you may have used them in other text editors such as [Notepad++][1] or [Sublime text][6]. If you have, then you already know how to use this extension.

Download
===============================

You can download the VSIX installer from the [Visual Studio Gallery][4].

How does it work?
===============================

After installing this extension, you will find a menu called `Text Macros` in the `Tools` menu.
It will only be visible when there is an active text or code editor.
It has 2 submenus, one that toggles the recording of a macro (Start/stop recording macro) and one that replays the last recorded macro (Playback macro).

 ![Screenshot][2]

So the idea is that you start recording, make some edits, stop recording, and then replay the edits.  
For example, here's what you would do if you just copied a few signatures from an interface that you have to implement:

 ![Demo][3]

You can change the shortcuts associated with the macro menus in Tools > Options > Environment > Keyboard.  
Look for the following commands:

 - Tools.ToggleMacroRecording
 - Tools.PlaybackMacro

What can be recorded?
===============================

Only text editing features can be recorded, so you cannot use this extension to automate work in, say, a Windows Forms editor.

Currently, here are the commands that can be recorded:

 - Cursor movements
 - Characters that you type
 - Tabs, new lines, deletions
 - Some text editing commands from the Edit menu (to lowercase, to uppercase...)

Change Log
===============================

**1.3 - Nov 28, 2013**

 - Fixed macros not working in certain file types (HTML...)
 - Recording additional edit commands: Format Document/Selection, Comment/Uncomment Selection,
   Delete Horizontal White Space, Increase/Decrease Line Indent, Organize Usings, Move Selected Lines Up/Down (VS 2013).

**1.2 - Oct 24, 2013**

 - Support for Visual Studio 2013
 - Added 'Ctrl+Shift+R' shortcut to match shortcut of previous Visual Studio versions

**1.1 - Feb 8, 2013**

 - Added visual cue while recording
 - Currrent macro now persists across sessions

**1.0 - Nov 13, 2012**

 - Initial version

Want to contribute?
===============================

 - Let me know of any issues you may find (include a portion of text and keystroke sequence if it is a problem with a macro)
 - Fork the code and contribute bug fixes or new features (ability to save a macro, for instance)

License
===============================

Text Macros for Visual Studio 2012/2013
Copyright (C) 2013 Xavier Poinas

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program. If not, see <http://www.gnu.org/licenses/>.

 [1]: http://notepad-plus-plus.org
 [2]: https://raw.github.com/xps/VSTextMacros/master/Documentation/screenshot.png
 [3]: https://github.com/xps/VSTextMacros/raw/master/Documentation/example.gif
 [4]: http://visualstudiogallery.msdn.microsoft.com/8e2103b6-87cf-4fef-9410-a580c434b602
 [5]: http://social.msdn.microsoft.com/Forums/en-US/vsx/thread/d8410838-085b-4647-8c42-e31b669c9f11
 [6]: http://sublimetext.info/docs/en/extensibility/macros.html
 
 [![githalytics.com alpha](https://cruel-carlota.pagodabox.com/ec90df53b58a3de3f98b8fbbc3a8c326 "githalytics.com")](http://githalytics.com/xps/VSTextMacros)
 
