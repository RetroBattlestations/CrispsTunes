This is the program for the **tenth** RetroBattlestations BASIC
challenge. I've never done a program that featured sound because of
difficulty creating sound on different platforms, but I felt it was
time! Since I've been working on Commander le Clef's Secret Encoder
Wheel (see link at bottom) I thought I'd write the program for the ZX
Spectrum first and it can be ported to other platforms from there.

The music notation format is based on [ABC
notation](http://abcnotation.com/wiki/abc:standard:v2.1).

For more details about the challenge, check out the post here:

  https://redd.it/hje132

## Porting ##

Before you start working on porting the program and changing things
work on your machine, try running the Spectrum 48k version in an
emulator (or real hardware if you are so inclined) so you can see how
the program works and what it sounds like. The Apple II version does
not make a good starting point because the Apple II does not have any
built-in commands and instead uses an assembly routine and a table
full of magic values to create the notes.

If your BASIC doesn't let you cheat and use the DIM command to clear
an array like the Spectrum does then look at lines 630-640 and 900-930
in the Apple II version for an alternative method.

The code is fairly simple and doesn't use any kind of dirty tricks but
it may be difficult to port depending on if your computer's BASIC
supports making sounds or if it requires some kind of assembly
routine.

See [List of Computers With On-Board BASIC](https://en.wikipedia.org/wiki/List_of_Computers_With_On-Board_BASIC)

## Enhancment Ideas ##

* Use graphics and make it display the notes
* Add a way to include lyrics that appear as the notes play so you can sing along
* Turn the keyboard into a piano and live play while pressing keys
* Support more of the ABC notation
* Chords/Polyphonic playback on machines that support it

## Typing Tips ##

When typing the program in you can leave off any lines which begin
with REM, they are not needed for the program to run. On many
platforms you can leave out the whitespace between keywords and
operators. IBM BASIC is not one of those however.

*Note*: On the TRS-80 Color Computer and BBC Micro you need to include
      the spaces around any IF, AND, OR, or THEN statement.

If you make a mistake and don't want to retype the entire line, most
of the BASICs have a way to make corrections.

### Amstrad CPC (464/664/6128/464+/6128+) ###

  On Amstrad CPC, use AUTO to start typing commands. Use the arrow keys
  to move about the line. Exit the AUTO mode py pressing Escape. You can
  also start on a specific line by entering AUTO 100 (for line 100).

  To go to the start or the end of the line use CONTROL+Arrow keys. You
  can also use SHIFT+Arrow keys to use the copy cursor. This is a second
  cursor that you move independendly, and will copy whatever is under it
  to the main cursor when you press COPY.

### Apple II computers ###

  On an Apple II+ use LIST <line number> to print the line with an
  error, then use ESC followed by A/B/C/D to move the cursor one step
  at a time. Position the cursor at the beginning of the line, then
  use the right arrow to move over the line and fix the error. Be sure
  to arrow all the way to the end of the entire line before you hit
  RETURN!

  On an enhanced Apple IIe, Apple IIc, or Apple IIgs you can also use
  ESC with the arrow keys. In 80 column mode (enter with PR#3) the
  cursor will change to a white block with a + in it, push ESC to drop
  out of movement mode.

### BBC Micro ###

  Use LIST <line number> to print the line with a mistake, then use
  the arrow keys to move up to the beginning of the line. Each press
  of the copy key will type in the character under the cursor. Make
  any necessary edits by just typing on the keyboard and using copy to
  avoid retyping everything.

### Commodore 64, Plus/4, and 128 ###

  Like the others, use LIST <line number> to display the line with
  problems, then use the arrow keys to move up and make any
  corrections. By pressing shift-INST you can insert a blank character
  if you missed something. Unlike the Apple II you don't need to arrow
  to the end of the line before pushing RETURN.

### IBM Cassette BASIC, Disk BASIC, Advanced BASIC, GW-BASIC ###

  Type EDIT <line number> and it will print the line on the screen and
  put your cursor at the beginning of the line. Arrow left/right and
  you can use Insert & Delete to make corrections. Like Commodore
  BASIC, you don't need to arrow to the end of the line before pushing
  RETURN.

### TI-99/4A Extended BASIC ###

  Type the line number and then arrow up (FCTN+E) and it will enter
  edit mode with that line loaded.  You can move within the line with
  arrow left (FCTN+S) and arrow right (FCTN+D) and move to the
  previous or next line with arrow up (FCTN+E) or arrow down (FCTN+X).
  You can delete the character under the cursor with DEL (FCTN+1) or
  turn on insert mode to insert extra characters with INS (FCTN+2).
  You do not need to move to the end of the line before pressing
  ENTER.

### TRS-80 model 100 ###

  This has to be the best built-in BASIC editor I've seen so far! Just
  type EDIT and the entire BASIC program will be loaded into the
  built-in word processor where you can make any changes you
  want. Press F8 to exit the editor and go back to BASIC.

### ZX81, Timex-Sinclair 1000, and ZX Spectrum ###

  Having a hard time finding where all the BASIC keywords are hidden?
  Get [Commander le Clef's Secret Encoder
  Wheel](http://retrobattlestations.com/Cmdr-le-Clef/Secret-Encoder-Wheel.pdf)
  with an alphabetical sorted listing of keywords and the secret
  keypresses required to enter them.
