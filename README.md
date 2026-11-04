# Silent Time Together Submod
A submod that let Monika read or use a laptop instead of staring (still she does it sometimes)
<img width="1440" height="798" alt="Captura de pantalla 2026-11-04 150021" src="https://github.com/user-attachments/assets/65aa96b9-2d9f-4316-b589-cd5282baaa5b" />


## What does this do?
- Instead of staring at you or your cursor, she will be reading or be at her computer
- The prompt is "Do you want to spend some silent time together?"
- She will ask you what are you going to do 
- New eyes: Six new eyes poses were added for the submod (three def and three leaning). There were made editing the default MAS eyes, but you are free to replace them (even you can replace them with your custom eyes of EmeraldBox submod)
  ```
  "eyes": {
    "z": "down"
    "x": "downright"
    "y": "downleft"
  }
  ```
- Animations: She will display different expressions and poses while she is focus (take your guess what she is doing or reading)
- If you place the cursor on her head, she will look at you
- Idle mode: It works like [return "idle"] (the time will change between day-noon-night, she can get and put away consumables (like coffee) and she can change her outfit if you have Auto Outfit Change submod)

# PLEASE READ BELLOW
## Conditions
- Affection points must be over 100
- She must have a book or a laptop. This submod includes the laptop of the image, but bellow I explain how to add more
- The book and laptop must be in the table_acs group (not cushion_book or others)

# Instruction
- Go to the "Releases" tab on the right this webpage and download "Silent Time Together.zip"
- Go to your MAS folder and merge the "game" and "characters" folders of the submod with yours

# How to add my own book or laptop?
Let's use as example Lisa's book by otter (if you want it, you can download it in Packs.zip here: https://github.com/Friends-of-Monika/otter-spritepacks/releases/tag/1.0.0)

Here it is the json file:

```
{
  "__author": "otter",
  "version": 3,
  "type": 0,
  "name": "acs_otter_lisa_book_tableacs",
  "img_sit": "otter_lisa_book_tableacs",
  "pose_map": {
    "default": "0",
    "l_default": "0"
  },
  "rec_layer": 2,
  "priority": 15,
  "acs_type": "table_acs",
  "stay_on_start": true,
  "select_info": {
    "display_name": "Lisa's book",
    "thumb": "otter_lisa_book_tableacs",
    "group": "table_acs",
    "select_dlg": [
      "Me, a grand mage? That was a long time ago, I'm just a humble librarian now."
    ]
  },
  "dlg_desc": "gift",
  "dlg_plural": false,
  "giftname": "otter_lisa_book_tableacs"
}

```
Now, to turn this book into a readable book, just add this line:
```
  "ex_props": {
    "book": true
  },
```
It will look like this:
```
{
  "__author": "otter",
  "version": 3,
  "type": 0,
  "name": "acs_otter_lisa_book_tableacs",
  "img_sit": "otter_lisa_book_tableacs",
  "pose_map": {
    "default": "0",
    "l_default": "0"
  },
  "ex_props": {
    "book": true        <--- Here
  },
  "rec_layer": 2,
  "priority": 15,
  "acs_type": "table_acs",
  "stay_on_start": true,
  "select_info": {
    "display_name": "Lisa's book",
    "thumb": "otter_lisa_book_tableacs",
    "group": "table_acs",
    "select_dlg": [
      "Me, a grand mage? That was a long time ago, I'm just a humble librarian now."
    ]
  },
  "dlg_desc": "gift",
  "dlg_plural": false,
  "giftname": "otter_lisa_book_tableacs"
}

```
In case you want to add a laptop, add this line instead:
```
  "ex_props": {
    "laptop": true
  },
```

# Credits
SzczawGirl who made the dialogues

# If you have any issue, please let me know
