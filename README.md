# drawsteelroll20
A character sheet for the (beta) Draw Steel ruleset for the Roll20 VTT

This is a pretty quick-and-dirty implementation of the MCDN Draw Steel Rules in the Roll20 interface.  I am NOT a professional programmer, and if you look too hard into the code you'll quickly figure out that I was sorta teaching myself CSS and Roll20 JavaScript on the fly.  Feel free to complain about how spagetti-like my code is because I will simply agree without comment.

To implement the character sheet in Roll20, do the following:

1.	Create a new game
2.	Under "Pick a Character Sheet", choose "Custom" from the list.

![image](https://github.com/user-attachments/assets/be5bf628-9ff4-4b3e-abc0-0ecd9a664cce)

3. Click "I'm ready, create game"
4. When the game home screen comes up, choose "Settings"
5. From the menu, choose "Game Settings"

![image](https://github.com/user-attachments/assets/08c703ad-b476-45b7-a798-dd8db3aa376e)

6. Scroll down in the page of settings until you get to the "Character Sheet Template" section.
7. Under that are a bunch of tabs.  We're only worried about the "HTML Layout" and "CSS Styling" tabs. Make sure the "HTML Layout" tab is selected.

![image](https://github.com/user-attachments/assets/ad9c304c-4acf-4f2e-96eb-b73e7bb84f7a)

8.  In another browser tab, open this repo, and click on and open the "drawsteel.html" file.

![image](https://github.com/user-attachments/assets/de89dc71-b2ac-4f0b-8c0e-2840bfb3acbd)

9. Copy all 1000+ lines of HTML code from the repo into the Roll20 HTML tab.  Feel free to grouse about how duplicative my templates are, and how a real programmer could have gotten the same results with about a third of the elements.  You're not wrong.
10. In the Roll20 page, click over to the "CSS Styling" tab.
11. Go back to this repo and open the "drawsteel.css" file.
12. Copy all the hundreds and hundreds of lines from the file into the "CSS" tab in Roll20.  If you are a professional CSS guy, you can feel super-righteous about how terribly my classes are named and organized.  Your hatred only fuels me.
13. Scroll down to the bottom of the Roll20 Game Settings page and click "Save Changes".  Roll20 will chug for a few moments and then toss you up to the top of the page.

![image](https://github.com/user-attachments/assets/8b4c08f3-6da3-46f1-b854-491ba9acbc4f)

14 Navigate back to your home page and launch your new game.

# Character Sheet Usage
Some quick notes:
1. Any bonuses in the "Kit" tab are automatically added to the appropriate "Action" rolls, so don't double-enter them (like they are in the Pre-Made character sheets in the Beta Packet); the code takes into account the damage type (melee, ranged, magic).
2. If you click the "Bane" or "Edge" box at the top of the sheet, it only stays until the next roll from that sheet; the +/-2 will be applied to the roll and then the Edge or Bane goes away.


# To-Do
1. Come up with a macro or code that will make DS-style Initiative work in Roll20.
2. Create a basic DS-style roll macro.
3. Create a simplified NPC Character Sheet
4. Get Resources and Victory counters to persist
5. Add Hero Tokens to the Character Sheet
6. Add support for double-edges and double-banes
7. Do some better stuff with the Background Tab
8. Figure out how to auto-populate a Free Attack entry into all character sheets.
9. Figure out a way to do generic DS rolls with proper crit-detection through a macro button.
10. See if an action button can be called from a macro
