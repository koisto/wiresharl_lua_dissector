# A Wireshark dissector

Based upon this tutorial:
https://mika-s.github.io/wireshark/lua/dissector/2017/11/04/creating-a-wireshark-dissector-in-lua-1.html

## Testing

Copy or symlink the lua file into wireshark's lua plugin directory.

Press Ctrl+Shift+L to make sure the dissector is reloaded whilst wireshark is running.

Server:
$ socat TCP-LISTEN:6789,fork stdout

Client:
$ telnet localhost 6789

