# My keyboard configuration

This repository contains my keyboard configuration for the [Dygma Defy](https://dygma.com/pages/defy) keyboard. I'm still getting used to it. So this is a work in progress and will be updated as I get more used to the keyboard and the layout.

I will give you my current configuration, but also some background on why I chose this layout and how I got there. I think this is important to understand the choices I made and to be able to adapt it to your own needs. I also saw **a lot** of keyboard designs and layouts while researching this, and was often annoyed by the lack of background information on why the layout was chosen the way it was.

Since a lot of the decisions I made for my keyboard layout were based on my personal preferences, I will start with some background information about myself. I'll keep it short though.

- I'm a software developer from Germany.
- My native language is German, but I also use a lot of English on a daily basis.
- I have been typing for over 20 years, but only recently started touch typing.
- My speed when touch typing on QWERTZ was about 50 wpm. Freestyling, looking at the keyboard every 10 to 20 characters, I got about 80wpm instead.
- I work as a software developer and type a lot of code in various programming languages like Python, JavaScript, C#, Rust and more.
- I'm also a gamer, but I don't play many competitive games.

## Physical keyboard

Having previously used a [Logitech G915 TKL] (<https://amzn.to/479JC5t>) with brown switches, I decided it was time to upgrade my keyboard to a more ergonomic design. I had no serious medical problems with my hands etc but I wanted to be proactive and avoid any problems in the future.

I now use the [Dygma Defy](https://dygma.com/pages/defy), a split ortholinear keyboard with 8 thumb keys on each side. It can be configured using the [Bazecor](https://github.com/Dygmalab/Bazecor) software, which offers quite a bit of customisation. My version has English keycaps and the Kailth Silent Brown switches. I am very happy with the keyboard so far.

## Windows Layout

Coming from a German QWERTZ keyboard, I also wanted to take the opportunity to change to a more ergonomic layout, especially as I'm a programmer and use a lot of special characters. I went down the rabbit hole and looked at [Dvorak](https://en.wikipedia.org/wiki/Dvorak_keyboard_layout), [Neo2](https://neo-layout.org/) plus its newer variants, [Workman](https://workmanlayout.org/), [EurKEY](https://eurkey.steffen.bruentjen.eu/), [Colemak](https://colemak.com/), [Colemak-DH](https://colemakmods.github.io/mod-dh/) and a few other layouts.

In the end, I decided to use [Colemak-DH](https://colemakmods.github.io/mod-dh/) because it seemed to be a good mix of ergonomics and support for both English and German. But unfortunately it seems that while a **lot** of thought went into the placement of the individual letters, the symbols and the symbol layer were not as well thought out and mostly remained in the QWERTY positions. My first idea was to use [EurKEY](https://eurkey.steffen.bruentjen.eu/) as my Windows layout instead. EURkey has the German characters **äöüß** on the **aous** keys on the AltGr layer, which is very easy to learn. It also has support for special characters that I used to have to remember the ALT codes for, like ·, ®, ©, ™ etc. Unfortunately, some of my client work requires me to use the US layout on a remote connection, so I decided against it and went with [English International](https://en.wikipedia.org/wiki/QWERTY#US-International) instead. This has drawbacks like the dead keys for single and double quotes, but I have found great workarounds for that (see below).

I thought about using [DreymaR's Big Bag Of Tricks / EPKL](https://github.com/DreymaR/BigBagKbdTrixPKL), but decided against it because I don't want to install additional software (with its own bugs) and there is no EPKL combination of the German layout for ortholinear keyboards as far as I can see.

## Keyboard Layout

Since [English International](https://en.wikipedia.org/wiki/QWERTY#US-International) is a pure QWERTY layout (just with special characters added), I used Bazecor to move the letter placement to match Colemak-DH. This is the layout I'm using now as my base layer.

### Key colors

To make learning easier, I have colour coded the keys. I use the colour palette from [Tailwind](https://tailwindcss.com/docs/customizing-colors). For reference, my keyboard brightness is set to 20 percent. The colours I use are:

- Keys without any functionality:
  - #000000
- Letter keys:
  - #0E7490 / Cyan 700:
- Destructive operations (Esc, Backspace, Delete):
  - #DC2626 / Red 600:
- Number keys (0-9):
  - #FB923C / Orange 400
- Modifier keys (Shift, Ctrl, Alt, OS):
  - #A21CAF / Fuchsia 700
- Function keys (F1-F12):
  - #E879F9 / Fuchsia 400
  - #FB7185 / Rose 400 (alternative)
- Navigation keys (Arrows, Mouse, Tab):
  - #FACC15 / Yellow 400
  - #FB923C / Orange 400 (alternative)
- Special keys like Print, Insert, Num Lock, ...:
  - #6D28D9 / Violet 700
- Multimedia keys
  - #E879F9 / Fuchsia 400
- Layer shift:
  - #15803D / Green 700
- Symbols:
  - #94A3B8/  Slate 400
- Space, Enter, Homing keys
  - #F8FAFC / Slate 50

I have not been too strict about the colour coding, sometimes I use a second colour to accentuate, e.g. the arrow keys in yellow 300 and the other navigation keys next to them in orange 400. Also the keys for e.g. switching to the symbol layer are in the same colour as the symbols themselves and not in the "layer" colour.

I use several layers on my keyboard:

1. Colemak DH
2. Navigation
3. Symbols
4. Gaming
5. Shift
6. Numpad
7. German Umlauts

### Base Layer (1)

This is the layer I use for typing. It is a Colemak-DH layout with the following changes:

- The number row has been completely replaced by the \[F1\] to \[F12\] keys. The numbers are now on the [symbols layer](#symbols-layer-3) instead. I made this change because I use the \[F*\] keys a lot in my work and I want to be able to reach them without having to use the layer shift.
- The only symbols left on the base layer are the comma \[,\], the dot \[.\] and the semicolon \[,\]. The rest are on the [symbols layer](#symbols-layer-3).
- Since I have \[<\] and \[>\] in an easily accessible and logical position on the [symbols layer](#symbols-layer-3), I wanted to have another value for the shifted state of \[,\] and \[.\]. Since this is not directly possible, I decided to use a separate [shift layer](#shift-layer-5) instead of the normal shift key.
- \[Esc\] is on the leftmost key of the top row (as usual). I put \[Del\] on the mirrored position on the right side. This feels quite natural coming from a QWERTZ keyboard. I had \[Del\] on the right thumb cluster next to \[Backspace\] before, but I found that I too often pressed it by accident.
- The [shift layer](#shift-layer-5) is reachable on both pinkies in the home row. I prefer to have it here instead of one row lower because it is easier to reach and I use it more often than the [symbols layer](#symbols-layer-3).
- The [symbols layer](#symbols-layer-3) has the same position as the shift layer, but one key lower. I have it on both hands as well, because the layer contains a lot of symbols on both hands.
- The German characters \[ä\] \[ö\] \[ü\] \[ß\] are accessible on an [umlaut layer](#german-umlauts-layer-7). This layer is accessible with the right little finger as an [OSL (One-Shot-Layer key)](https://support.dygma.com/hc/en-us/articles/360007166377-What-are-One-Shot-Modifiers-and-One-Shot-Layers-).
- I have a Superkey "CCP" (Copy / Cut / Paste) which does exactly that:
  - Tap: Copy
  - 2x Tap: Cut
  - Hold: Paste
- The \[Print Screen\] key is on the base layer as well, because I use it quite often and like that it is easily accessible.
- I also have a Superkey "Layer" which for now mainly has the functionality to bring me back to the base layer from whereever I are if I accidentally ended up somewhere else. I also activate the [gaming layer](#gaming-layer-4) with it.
  - Tap: [Base layer](#base-layer-1)
  - 2x Tap: [Gaming layer](#gaming-layer-4)

Two spots are still free, I'm not sure what to put there yet and don't want to clutter the layout with something only rarely used.

Thumb keys:

- This has gone through several iterations. I find it very hard to accurately hit the thumb keys, so I have tried not to overload this.
- Left hand
  - I have only ever used the left hand for space and the modifier keys on QWERTZ, so I decided to keep it that way.
  - Space is the most important key, so it got the "home" left thumb key.
  - \[Alt\] and \[Ctrl\] are next to it, so they are easily reachable.
  - Below \[Alt\] and \[Ctrl\] I have the shifted versions of those (\[Alt+Shift\] and \[Ctrl+Shift\]). I find it easier to only have to press one key instead of two for those modifiers and they are used quite often in various applications like editors and IDEs.
  - \[Win\] takes the place that is the hardest to reach because I use it least often.
  - The big thumb button has an [OSL (One-Shot-Layer key)](https://support.dygma.com/hc/en-us/articles/360007166377-What-are-One-Shot-Modifiers-and-One-Shot-Layers-) that activates the [navigation layer](#navigation-layer-2). I had it on another position before, but I find it easier to blindly hit it here to access the navigation layer more quickly.
  - The remaining left thumb key has an [OSL (One-Shot-Layer key)](https://support.dygma.com/hc/en-us/articles/360007166377-What-are-One-Shot-Modifiers-and-One-Shot-Layers-) that activates the [numpad layer](#numpad-layer-6).
- Right hand
  - \[Backspace\] is also often used, so it got the "home" right thumb key.
  - The space left to it is unused for now because I too often press it accidentally.
  - \[Enter\] on the big thumb key.
  - The arrow keys in the usual layout ("WASD" like, not "HJKL"). This is experimental, I might remove them in the future and only rely on the navigation layer. But for now I find it easier to use them here sometimes. Not really decided on this.
  - \[Ctrl+Alt\] on the remaining right thumb key. This is used only rarely (especially with the [symbols layer](#symbols-layer-3) being present), so it's okay that it's a bit harder to reach. I use it mostly for autofill \[Ctrl+Alt+A\] in [KeepassXC](https://keepassxc.org/).

### Shift Layer (5)

This layer complements the [base layer](#base-layer-1). Most of the keys are the same as they are there, but with an added "shift" modifier. The following keys are different:

- The comma \[,\] has the single quote \['\] as its shifted state. This makes for a very convenient way to type the common English contractions with "n'" like "don't", "can't", "won't" and even better for "I'" like "I'm", "I'll", "I'd" etc. Also \['\] almost looks like \[,\], so it's easier to remember.
- The dot \[.\] has the double quotation mark \["\] as its shifted state. I previously had the single quote here, typing "I'" was too cumbersome.
- The semicolon \[;\] currently has no shifted state because \[:\] is available on the [symbols layer](#symbols-layer-3). I might put something here in the future.
- In the English International keyboard layout, some keys are dead keys. I cannot stand this at all, so whereever I use these keys I actually instead have a macro that types the key followed by a space. I affectionately call these "Undead" keys. I use them for single quotes \['\] and double quotes \["\] here and for the backtick \[`\], tilde \[~\] and circumflex \[^\] on the [symbols layer](#symbols-layer-3).

### German Umlauts Layer (7)

This means that when I press my right pinky, the layer is activated until I press another key. This way I can type the German characters without having to hold down the key. Having them in the same position as the characters without the dots is very intuitive and easy to learn.

### Symbols Layer (3)

I took heavy inspiration from [Getreuer's layout](https://getreuer.info/posts/keyboards/symbol-layer/index.html) for this layer. It is (imho) the best symbols layer on the internet with a lot of thought put into the placement of the symbols. I only made some very small changes to it, to accomodate the fact that my base layer has other symbols on it then his.

I also added keys for \[En Dash\] (–) for my typographic satisfaction and the \[Nbsp\] (non-breaking space) for my programming needs.

If you want to tweak it to your needs, [Xah Lee's page on char distribution](http://xahlee.info/comp/computer_language_char_distribution.html) is a useful resource for the distribution of symbols in various programming languages.

### Navigation Layer (2)

This layer is used for navigation.

Mouse navigation:

- The mouse movement is controlled with the left hand in a "WASD" like layout.
- The mouse wheel also is on this hand next to the mouse movement keys.
- The "Back" and "Forward" buttons are rarely used together with mouse movement, so they are on the left hand as well.
- The "Left click", "Right click", "Mittle click" mouse buttons are on the right hand to make it easier to move the mouse while also holding down a button.

Cursor navigation:

- The cursor movement is controlled with the right hand in a "WASD" like layout.
- To the left is an added \[Ctrl+Left\] key for jumping to the beginning of a word. To the right is an added \[Ctrl+Right\] key for jumping to the end of a word.
- The "Home", "End", "Page Up" and "Page Down" keys are placed next to the cursor movement keys.

Other keys:

- The right thumb cluster has no navigation keys here as it would be duplicating those.
- On the right hand, I also have the media keys \[(Play/Pause\], \[Next\], \[Previous\]) and the \[Mute\] key and it's kind of "navigating music" (yes, that's a bit of a stretch), so I put them here as well.

### Gaming Layer (4)

This layer tries to resemble QWERTY as much as possible, so for gaming I don't have to remap the keys in the game.

Notable key placements:

- The number keys on the left hand are extended downwards up to 8, so I can reach mor "hotbar" keys with my left hand.
- \[Shift\], \[Ctrl\] and \[Alt\] are placed so they resemble the positions on a classic keyboard. Games often rely on pressing one of those as a modifier for various actions, so I wanted to have them accessible is the usual positions.

Problems:

The "WASD" feels unnatural because of the ortholinear shifting. I'm thinking about shifting all the keys one column to the right, so these keys are on the "home row" instead. But I'm not sure how to best place \[Shift\] and \[Ctrl\] for that. I think they would need to be shifted one row to the right as well, but then "TGB" would have to be put on the leftmost column. It might work, depending on the game and how the keys are used there.

An alternative would also be to remap games to use "ESDF" instead of "WASD", but I'm not sure if that would be worth the hassle.

I guess I'll have to try these possibilities out for a while and see what works best.

### Numpad Layer (6)

This layer is used for the numpad. I use it mainly for entering numbers, but also has the usual \[+\] \[-\] \[*\] \[/\] and \[Num Enter\] key. The \[0\] and \[.\] keys are on thumb cluster, quite conveniently placed almost as they would be on a normal numpad.

The \[Numlock\] and \[Insert\] keys are also on this layer, but I rarely use them.

I placed the numpad on the right hand because I'm used to it and can easily type numbers from muscle memory. The left hand is basically unused for now.

## Learning the new layout

I used [Typingclub](https://www.typingclub.com/) to learn the letter positions. To really nail down the basics I later used [keybr.com](https://www.keybr.com/) to focus on getting my fingers up to spead and [monkeytype.com](https://monkeytype.com/) for a more realistic typing experience. I put in some chapters of [Alexander Wales' Worth the Candle](https://archiveofourown.org/works/11478249) I was reading at the time and typed it out to get used to the new layout.

## Other alternatives for Dygma Defy layers

- [objectmanip's layout](https://github.com/objectmanip/Dygma-Defy-Layers)
  - A Colemak-DH layout with a lot of super keys and 8 layers, including 3 gaming layers. Brackets split between left and right hand. Shift on the left pinky only. Control as well. Arrow keys on the main layer. Thumb cluster is used for various things (besides space, enter and backspace): Layer shift, media keys, and more super keys.
- [tarbari's layout](https://github.com/tarbari/defy_layers)
  - A variant of Colemak-DH with some national characters added. Enter on the left pinky. Uses "home row modifiers" for OS, Ctrl, Alt and Shift. Thumb cluster used for layer shifting mainly. 8 layers.
- [Obskyur's layout](https://github.com/Obskyur/Dygma-Defy__Profiles>)
- [barlevalon's miryoku based layout](https://github.com/barlevalon/dotfiles/blob/main/dygma/miryoku-qwerty/README.md)
