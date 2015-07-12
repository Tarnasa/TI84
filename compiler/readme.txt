-----------------------------------------
The TI-Basic Compiler
Matthew Iselin
-----------------------------------------

Changes in this version, 1.2, are in 'change.log'.

-----------------------------------------

Thankyou for taking the time to download the TI-Basic Compiler. If you enjoy creating games on your calculator, or want to create a formula list for an exam, or even want to just improve your productivity, the TI-Basic Compiler is for you. Before you can use it, though, a quick run through of how to use the compiler is necessary.

To compile a file, all you have to do is create the file, with a 'tib' extension (without this, the compiler will complain). If you can't see extensions, go to Tools->Folder Options->View, and then uncheck 'Hide extensions for known file types'.

Once you've written your code, you have two options: drag your file on top of the 'tibasic.exe' file, or (the preferred way) to use a command line. Don't be daunted by this concept, as command lines are really not all that difficult.

If, for instance, your code is in a folder on your desktop, you would use the following command line:

C:\tibasic\tibasic.exe "C:\Documents and Settings\[username]\Desktop\[folder]\[filename]"

Simple, isn't it? You can even copy from the address bar in Explorer and paste into the command line for even quicker compilation.

-----------------------------------------

This is an example source which you can use to test that the system is working. Copy the following into a file, compile the file and then send to your calculator:

Disp "Testing:"
If 1=1:Then
Disp "Good!"
End
Disp "Works!"

The above should print out, on 3 lines, "Testing:", "Good!", and "Works!".

-----------------------------------------

There are two extra switches that can be used on the command line, for advanced users only. One is the '-v' option, and must be AFTER the filename itself. This enables verbose output, allowing you to view microsecond timing for the compilation.

The other is the '-d' option, and decompiles the program into TI-Basic code. Note that the program must not be a compiled assembly program (decompilation of such files returns garbage output).

-----------------------------------------

There are a few symbols that could not be directly transferred to the language and were replaced instead with simpler tokens. Also note some of these are 'shorthand' versions of supported tokens:

& --> 'and'
| --> ' or '
~ --> ' xor '
theta --> '[theta]'
powers --> '^' (for instance, 5 squared would be '5^2')
'e' constant --> '[e]'
Store --> '->' (same for such things as >DMS: ->DMS)
Roots --> '[root]^' (for instance, square root would be '[root]^2')

All Picture variables (Pic0 - Pic9) and String variables (Str0 - Str9) are CAPITALIZED (ie. STR0)

Other shorthand versions for more obscure functions exist, to find these the source code is viewable (CVS Browse on the SourceForge page).

-----------------------------------------

As a final note, all support requests must go to either the 'Support Requests' tracker on the SourceForge page, or pcmattman@gmail.com (the email method usually gets a reply within 24 hours). The trackers are checked often so you can be assured that your request for help will be responded to.

Happy programming!