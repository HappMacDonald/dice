# dice
🎲 Javascript D&amp;D style dice app with good entropy

This was a code sprint to develop an application similar to https://www.wizards.com/dnd/dice/dice.htm
But:
* Prettier
* With better entropy (they use a weird custom PRNG seeded by current time, I use window.crypto.getRandomValues() which is a newer standard)
** That's actually the original motivation for making this, two people rolling dice together over chat aren't going to be fed the same values.
* And a few extra nice features.
** Mine allows rolling all specified dice at once (zero qtys blanks out all dice so you can only add the ones you need).
** Mine totals all rolls presently on screen, either if you are rolling all or rolling one after another manually.
** Mine uses HTML Number inputs so that invalid values cannot be entered, you get handy "spinner" arrows on each field, etc.
** All outputs on my app allow select-on-click — and if the browser handles it properly — copy-to-clipboard-on-click for convenience.
** Modifier sign widget is far easier both to read and to operate.
** Mine allows partial resets (reset inputs, clear rolls, and clear history) in addition to full page reset.
** I threw in d2 = "coin" on a whim, so that one would not have to resort to dx for a simple coin flip. 😋
** My UI presents as a comfortable size on modern 1080p PC monitors and smartphones alike.
** Bigger friendlier interface elements to hit with the mouse.
** My code is way less redundant (DRY principle) and easier to maintain.

Presently in beta, I'm having my friend who wanted the danged thing in the first place try it out so we'll see how it goes. ;)
