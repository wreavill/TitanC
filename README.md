# TitanC
Titan, written in C++

Titan (Precompiled) will still send notifications about snipes to us (the Vortex team).
Since I know some guy is going to spam the private snipes webhook, I've removed it from source code... (that isnt enough though and I know it).

Some backstory:
It all started last summer, back when Vortex was called Ascension. We were working on a new sniper called (not surprisingly) - Ascension Sniper. It was a complete piece of crap and I scrapped it. After moving over to Vortex, I rewrote the sniper again and called it Titan. It was a lot faster than Ascension Sniper because I used a different module to send requests... but it still wasn't good enough. After that, I wrote Titan in C++... and here we are today. It was good for a brief moment, and then it fell into the shadows again. I've had enough of working on the sniper and instead of keeping it for myself and teasing people, I decided to release the source code to public. Use Titan while you can, because Roblox will most definetly fix the (bandwidth eating) price check method.


Copy the rapidjson from here: https://github.com/Tencent/rapidjson/tree/master/include
to the TitanRewrite directory

To compile under linux, run the command:
g++ CSniperThread.cpp CTokenCacher.cpp mainfuncs.cpp rblx.cpp TitanRewrite.cpp -I/usr/include/libxml++-2.6 -I/usr/lib/x86_64-linux-gnu/libxml++-2.6/include -I/usr/include/libxml2 -I/usr/include/glibmm-2.4 -I/usr/lib/x86_64-linux-gnu/glibmm-2.4/include -I/usr/include/glib-2.0 -I/usr/lib/x86_64-linux-gnu/glib-2.0/include -I/usr/include/sigc++-2.0 -I/usr/lib/x86_64-linux-gnu/sigc++-2.0/include -lxml++-2.6 -lxml2 -lglibmm-2.4 -lgobject-2.0 -lglib-2.0 -lsigc-2.0 -lssl -lcrypto -pthread -lgmp -lcrypt -lm -lcurl -std=c++11 -U__STRICT_ANSI__