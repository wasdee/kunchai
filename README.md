# kunchai
a phonetic input method for Thai. Also known as, a Thai transliteration keyboard. a Thai IME.
![Google Input Tools](Assets/Animation.gif)

# Pain Point
1. I don't want to buy a thai+english keycap for my mechanical keyboard. English keycap is light lit thru is so beuatiful. the thai keycap is opaque.
2. I'm not able to spell many common thai words without mistake. 
3. I'm a faster typer on English

# existing projects
1. Google Input Tools - this is only works on chrome-based browser.
2. [Pim Thai Dai Laew: You can now type in Thai!](https://blog.google/around-the-globe/google-asia/pim-thai-dai-laew-you-can-now-type-in/)
3. <https://www.lexilogos.com/keyboard/thai.htm>


# Questions 
0. Could we just use Google Input Tools?
Maybe, but it's not open source. It might be done by reverse engineering the browser extension.

1. How to use windows language service? 
They are called [Input Method Editors (IME)](https://learn.microsoft.com/en-us/windows/apps/design/input/input-method-editors).
They requires you to access  `Text Services Framework (TSF)`. Normally, api are in c/c++.

1. Could we communicate with windows language service using Python?
Yes, pls try <https://github.com/EasyIME/PIME> It looks mature and updated.

1. How to Install Python Exe? Best exp is here. <https://github.com/timmo001/system-bridge>
2. What is the good enough way to translate a set of English char to Thai pharse?
3. Are there any karaoke database that we can use?
Nope. But, we can use `pythainlp` to build our own dataset.

1. Could we build an AI model to do this?
Maybe, but that is beyond my knowledge.

