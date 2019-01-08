# university-sniffer
Course: Computer networking workshop.  
Project: A network Sniffer

The assignment was to build a network Sniffer supporting common protocols.
I decided it would be a good opportunity to try out WinPcap.
To make things simple - I decided to "copy" the UI from Wireshark and I used 
http://frhed.sourceforge.net/en/ for the hex viewer.

I think this is a good sample for understanding how to work with WinPcap and
the basics of writing a network sniffer.
Some optimizations could be made, specifically where with the conversion of the
packets to UI components.

I used VS2010 and the UI was written in MFC (not too popular these days, but it
made the development go faster).
The sniffer and network code itself aren't based on MFC and so the code can be
used in any C++ project (console/lib/qt etc...)

When reviewing the code - a good starting point would be: MainFrm.h/MainFrm.cpp

# Screenshots

![Protocols](/docs/screenshots/protocol-filter.jpg?raw=true "Protocols")
![DNS and ICMP in action](/docs/screenshots/ping.jpg?raw=true "Ping")
