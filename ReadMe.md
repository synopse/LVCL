LVCL - Light VCL
================

(c) 2008-2019 Arnaud Bouchez - Synopse

'Light VCL' - as its name states, is a "light" version of the VCL Delphi library.

It's compatible with DFM forms: just extract in some directory, put this LVCL directory in your Project/Options/Path/SearchPath directory list (to override standard Borland library), and your .EXE will shrink from 300KB to 30KB... 

Perfect for some programs (installation, server, background tool...)

That’s no magic, only optimization to the only-needed features of a minimal Delphi application!

Foreword:

- By design, only change LVCL existing properties in your DFM, otherwise you'll get error on startup.
- Currently compiles on Delphi 7 (2007?) only.
- This source is based on [VCL Light by Paul Toth](http://tothpaul.free.fr/sources.php?lvcl.lvcl1), from which we took the principles and just went further.


Notes about SysUtils.pas:

- Some routines are improved/faster than original;
- Simple but sufficient TThread support;
- Dates have a fixed format: 'YYYY/MM/DD hh:mm:ss';
- format() supports %% %s %d %x %.prec? %index:?
- Cross-Platform: Windows or Linux (via Kylix, only RTL, not the GUI).
 

Notes about Classes/Controls/ExtCtrls/Graphics/Forms:

- compatible with the standard .DFM files;
- only use existing properties in your DFM, otherwise you'll get error on startup;
- TForm can be easily minimized to tray;
- Implements TButton, TCheckBox, TEdit, TLabel, TMemo, TBrush, TCanvas, TFont, TPen, TPicture, TImage, TStream, TMemoryStream, TResourceStream, TReader, TList, TStringList.

More details are available in the source code.

The *Secure Notepad* Demo uses LVCL - don’t forget to take a look at its source in https://github.com/synopse/LVCL/tree/master/Demo/MySecNotepad !