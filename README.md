# Puller

Puller is an addon for FFXI / HorizonXI / Ashita v4 that enhances the puller role experience by sharing mob details directly in party chat. If you're familiar with the **Checker** addon, **Puller** will feel similar but with the added benefit of broadcasting the entire Checker mob details to your party during a pull. No more yelling in voice chat that "this one is Incredibly Tough!"

---

### TL;DR

Target a mob and use `/pull` to notify your party with details about the mob you're pulling back to them.

---

### Compatible with the Checker Addon

Puller works perfectly alongside the Checker addon, though it doesn't require Checker to function. Checker shows mob stats like name, level, difficulty, evasion, and defense when you use `/check`. Puller extends this functionality by sharing all of those details with your party when you're ready to pull, allowing everyone to stay updated on the mob’s Checker information.

---

### Install

1. Download `puller.lua` from [Github](https://github.com/AddonsXI/Puller/blob/main/puller.lua).
2. Navigate to your FFXI `Game > addons` directory.
3. Add a new folder called "puller".
4. Inside of the newly created folder add the `puller.lua` file.

*Note: You should have a single folder named "puller" containing `puller.lua` in the `Game > addons` directory.*

---

### Load

1. To load the addon manually, type `/addon load puller` in-game.
2. To have it load automatically on game launch, add it to your default script. (Make sure to read the warnings included in the default.txt file)

![Puller Config](https://i.imgur.com/OoeejbM.png)

---

### Commands

- **`/puller`**  

  Opens the configuration menu for customizing settings where you can:
  - Choose an optional sound from the list of 21 `<call>` sounds to play for your party members during pulls.
  - Save or reset your settings to defaults.
  
- **`/pull`**  

  Add the `/pull` command to your standard pulling macro or type it in chat while targeting a mob to share the mob's name, level, difficulty, and attributes in party chat.
  
---

### Macro

Easily integrate the `/pull` command into your standard pulling macro.

```
/pull
/ja "Provoke" <t>
```

![Puller Example Macro](https://i.imgur.com/ySesqht.png)

---

### Walkthrough

1. **Check Mob** 

    Use the standard checking practice until you find the mob you have decided to pull back to your party.

2. **Target Mob** 

   Make sure the mob you intend to pull is targeted before using the `/pull` command in your macro.

3. **Use Pull Macro**  

   When you're ready to pull, simply use your pull macro!

   Make sure to have a line to your pull macro that contains only `/pull`.

4. **Broadcast to Party**  

   When `/pull` is triggered on a targeted mob, Puller will broadcast the following mob information in party chat:

    - Mob Name and Level
    - Difficulty: Displays mob toughness (e.g., "Too Weak", "Tough").
    - Attributes: Displays if the mob has high/low evasion or defense.
    - Optional Call Sound: Set a customizable alert sound to play during pulls.

---

### Potential Roadmap
- Message Customization
- Exp Chain Timer

[https://github.com/AddonsXI](https://github.com/addonsxi)
