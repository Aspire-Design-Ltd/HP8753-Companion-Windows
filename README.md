This is a windows version of the HP8753-Companion.

The project uses the Eclipse IDE.

To run the code you will find a executable in the bin directory. You need to download the repository and keep the directory structure the same.

You also need to install the National Instruments drivers (https://www.ni.com/en/support/downloads/drivers/download.ni-488-2.html#484357). The driver used for testing was the oldest 17.6 version to ensure it worked with the older USB interfaces.

This has been tested using the GPIB-USB-HS, GPIB-USB-B interfaces with a HP8753ES VNA.


To build the code you will need:
1) Eclipse with the CDT extentsion.
2) GTK and minGW64 need to be installed using the MSYS2 software. Use the instructions from https://www.gtk.org/docs/installations/windows/
3) Ensure you have the National Instruments drivers installed.
4) You should now be able to import the project into your Eclipse IDE and compile.

Modifications to the original Linux code have been highlighted with a comment "Windows Mod"


NOTE: the GTK port for windows insists that you have a base directory and the executable is in a sub directory called "bin". You also need all the dll's included. In addtion the "lib" and "share" directory need to be included in the base directory.

Note Eclipse will compile the executable into the "debug" directory. You need to copy this compiled code into the "bin" directory where you can debug the the code using the GDB debugger.

FINALLY. To connect to your VNA you need to click the 'Use Card Index and ID' click box.

The 'Analyze Learn String' does not work.

All the 'Get Trace', file download and PDF documentation works.

FINAL FINALLY: The sqlite3 data base is saved at C:\\Users\\"you user name"\\AppData\\Roaming\\hp8753c in a data base file hp8753c.db

FINAL FINAL FINALLY: The logging part has not been used or tested. Enjoy.





