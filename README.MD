# My keyboard configuration

## Physical keyboard

Previously coming from a [Logitech G915 TKL](https://amzn.to/479JC5t) (brown switches), I decided it's time to upgrade my keyboard to a more ergonomic design.

Now I use the [Dygma Defy](https://dygma.com/pages/defy), a split ortholinear keyboard with 8 thumb keys on each side. It can be configured with the [Bazecore](https://github.com/Dygmalab/Bazecor) software. My version has English keycaps and the Kailth Silent Brown switches.

## Windows Layout

Coming from a German QWERTZ layout, I also wanted to use the opportunity of switching the keyboard to also change to a more ergonomic layout, especially since I'm a programmer and use a lot of special characters. I went down the rabbit hole and looked at [Dvorak](https://en.wikipedia.org/wiki/Dvorak_keyboard_layout), [Neo2](https://neo-layout.org/) plus its newer variants, [Workman](https://workmanlayout.org/), [EurKEY](https://eurkey.steffen.bruentjen.eu/), [Colemak](https://colemak.com/), [Colemak-DH](https://colemakmods.github.io/mod-dh/) and quite some other layouts.

In the end, I decided to go with Colemak-DH, because it seems to be a good mix of ergonomics and support for both English and German writing. But I absolutely couldn't stand the placement of the special characters, so I decided to go with EurKEY instead as my Windows layout. EURkey has the German characters **äöüß** on the **aous** keys on the AltGr layer, which is very easy to learn. Also it has support for special characters I previously had to remember the ALT codes for, like ·, ®, ©, ™ etc. Almost every character is available somewhere, so it can be easily remapped to easier accessible keys in the Bazecore software.

I thought about using [DreymaR's Big Bag Of Tricks / EPKL](https://github.com/DreymaR/BigBagKbdTrixPKL), but I decided against it because I don't want to have to install additional software (with it's own bugs) and also there is no EPKL combination of the German layout for ortholinear keyboards, as far as I can see.

## Keyboard Layout

Since EurKEY is a pure QWERTY layout (just with improved special character placement), I used Bazecore to move the letter placement so that it matches Colemak-DH. This is the layout I'm using now as my base layer.

The functions color coded and use the [Tailwind](https://tailwindcss.com/docs/customizing-colors) color palette:

- 000000: Off
- Red 600 / #DC2626: Esc, Backspace, Delete
- Orange 400 / #FB923C: Numbers
- Fuchsia 700 / #A21CAF: Modifier keys (Shift, Ctrl, Alt, OS)
- Cyan 700 / #0E7490: Letters
- Yellow 400 / #FACC15: Navigation keys (Arrows, Mouse, Tab)
- Violet 700 / #6D28D9: Function keys (F1-F12), Print, Insert, Num Lock
- Green 700 / #15803D: Layer shift
- Slate 400 / #94A3b8: Symbols
- Slate 50 / #F8FAFC: Space

I was not too strict about the color coding, sometimes I use a different color as an accent, e.g. having the arrow keys in Yellow 300 and the other navigation keys next to them in Orange 400.

I use several layers on my keyboard:

1. Base layer
2. Navigation and Numpad
3. Symbols
4. Gaming
5. Layer Shift / Utility

### Base Layer

This is the layer I use for typing. It is a Colemak-DH layout with the following changes:

- Minus in the "German" position (where it is on QWERTZ), replacing the question mark (which is now on the symbols layer)
- The German characters äöüß on the keys in the middle of the keyboard. These can easily be replaced with characters from another language, if needed.
- Single and double quotes, replacing the semicolon (which is now on the shift layer on the comma key) and the colon (which is now on the shift layer on the period key).
- The symbols on the number row are not usable anymore, since they have been moved to the symbols layer. Shift + number row are the F keys instead.
- The numbers are split after the 6, so that in the F key usage everything fits in the top row.

Besides that:

- I type space with my left thumb, so it got the "home" left thumb key.
- Backspace on the right "home" thumb key.
- Enter / Control on both big thumb keys.
- OS and alt on both bottom thumb rows.
- Shift on both pinkies.
- Layer shift to the symbols layer also on both pinkies.
- Layer shift to the navigation and function layer on both innermost thumb keys.
- The keys next to space and backspace are unused for now to avoid accidental presses. Might be used for something in the future when I get more used to the keyboard.

### Navigation and Function Layer

This layer uses some of the concepts of Neo2

### Symbols Layer

I took heavy inspiration from [Getreuer's layout](https://getreuer.info/posts/keyboards/symbol-layer/index.html) for this layer. It is a very well thought out layer with a lot of thought put into the placement of the symbols. I made some changes to it, though, to accomodate the fact that my base layer has other symbols on it.

See [Xah Lee's page on char distribution](http://xahlee.info/comp/computer_language_char_distribution.html) for the distribution of symbols in various programming languages.

### Numpad Layer

### Gaming Layer

### Layer Shift / Utility Layer

## Learning the new layout

I used [Typingclub](https://www.typingclub.com/) to learn the letter positions. To really nail down the basics I later used [keybr.com](https://www.keybr.com/) to focus on getting my fingers up to spead and [monkeytype.com](https://monkeytype.com/) for a more realistic typing experience. I put in some chapters of [Alexander Wales' Worth the Candle](https://archiveofourown.org/works/11478249) I was reading at the time and typed it out to get used to the new layout.

## Other alternatives for Dygma Defy layers

- [objectmanip's layout](https://github.com/objectmanip/Dygma-Defy-Layers)
  - A Colemak-DH layout with a lot of super keys and 8 layers, including 3 gaming layers. Brackets split between left and right hand. Shift on the left pinky only. Control as well. Arrow keys on the main layer. Thumb cluster is used for various things (besides space, enter and backspace): Layer shift, media keys, and more super keys.
- [tarbari's layout](https://github.com/tarbari/defy_layers)
  - A variant of Colemak-DH with some national characters added. Enter on the left pinky. Uses "home row modifiers" for OS, Ctrl, Alt and Shift. Thumb cluster used for layer shifting mainly. 8 layers.
- [Obskyur's layout](https://github.com/Obskyur/Dygma-Defy__Profiles>)
- [barlevalon's miryoku based layout](https://github.com/barlevalon/dotfiles/blob/main/dygma/miryoku-qwerty/README.md)
