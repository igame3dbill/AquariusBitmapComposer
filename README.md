-- Aquarius Bitmap Composer
-- development version 1.0.0.1
-- MODIFY AND EXPORT 8 BIT CHARACTER DATA
-- December 4 2013 Public Domain Open Source

Export options-

White with Alpha, Black with Alpha, Inverted White with Alpha.
Exports to png in folder path of the application or stack "/Images/" & the size of the images & the choice 
Will export 256 images at a go.
-- remind me to make a requester.

Keyboard commands.
Arrow keys scroll the current character in the array
Tilde and Tab keys move back and forth through the character set list, applying any changes.

Space, Return, and keypad Enter are redunant apply buttons --to be changed.

Command key on the Mac, Control key on windows AND
S 	save a text file representing the graphics as binary bits, ie, "0101010" 

O	Open a text file that contains lines of sixty four 1s and 0s representing graphics characters

C	Copy current graphics

V	Paste the black of the graphic in memory

Z	undo, i think i broke this.

About the livecode stack AquariusBitMapComposer_MainStack
-- For use in Livecode stack script.
-- works in livecode 6.0.2 (breaks after that)
http://downloads.livecode.com/livecode/6_0_2/
-- This script references a substack "CharacterNumList" with two fields "CharacterNumField" and "MenuInListField"
-- This script overuses stack (the mainStack of this stack) and the costum properties need cleaning up.
-- createEightBitGrid generates the graphics the user will paint pixels with.
-- mouseDown, mouseStillDown, and mouseDragCheck handle painting
-- commandKeyDown handles the usual program shortcuts
-- ClickFieldPick is a lazyman's menu system taking imput from "MenuInListField" of stack "CharacterNumList"
-- ig3d_SaveBitmapwithAlpha does some kind of magic to export images with alpha channels
