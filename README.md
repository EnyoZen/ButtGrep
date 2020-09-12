# ButtGrep
Buttgrep is a small Python program that interacts with Intiface Desktop to parse real time log files. (It makes toys vibrate to games and programs)
It came out of looking at the effort of people to integrate FFXIV with Initface using custom branches of ACT and Triggernometry. I kinda went "But... logs" and then went "But... I can use this for *anything* with logs..." and... ButtGrep. 

**I am not a great coder. I'm admitting that now. Feel free to modify and use this for whatever, within the license and share your modifications back to us.**

In essence, the program asks for a log file to follow. This can be any cleartext that it can read, preferably something updated in realtime by another program. 
The program then asks for a .ini file that contains a list of "trigger" phrases and timing and intensity values. 

Assuming you have Initface Desktop running it connects as a client and then begins reading new entries to the file and comparing them against the ini. 
Then if it finds a match it sends information to Initface to vibrate a toy based on it. 

Current limitations: 

  **1.** Because of the way everything is written, the commands overlap. This means if you set off a trigger that should last 5 seconds and then one that should last 1 second, the command after 1 second is going to turn everything off. I don't have a good solution for this without making it way more complex and for my uses this is a good thing because it avoids having stacked commands. 

  **2.** Only one toy at a time. This should be fixable but I haven't gotten around to it. 

  **3.** Only vibration: This is super simple to fix but I only own vibrating toys and don't have any way to test linear or rotation motions. 

  **4.** Currently this only uses one set of files at a time. I have plans to expand this so that I can have it run against two sources. 

  **5.** If your BT connection drops sometimes you'll need to bounce Initface and relaunch Buttgrep to get things going again. BT is Radio. Radio does not transmit well through booty. 

Lastly, there's a setup video to use this with FFXIV. It's not well done. I didn't script it. It's just to get everyone started. 
https://www.youtube.com/watch?v=SzJKAATBbiQ

I'm trying to clean up my social media threads between my directly porny stuff and my dev and 3D printing stuff. I'll put random blog posts about this over at my Ko-fi but ButtGrep won't ever go "for pay" for the app. If you want to tip or support my weird projects like this then thanks and that's the place to do it, but not expected or required: https://ko-fi.com/enyozen/posts
