# Wordle Bot
A Discord bot that allows users to play a game of wordle with features.

**Setup:**

Hosting on [Replit](https://replit.com/)

To host on Replit, create a new Repl and paste ```main.py```, ```wordlist.txt```, and ```alive.py``` in OR import the project in from Github (there are only 2 files). Running the program should activate the bot. To host it use the ```keepAlive()``` function (default enabled).

Hosting locally

To host the program locally, clone the repository OR paste in ```main.py``` and ```wordlist.txt```. Running the project should activate the bot. You can disable the ```keepAlive()``` function by commenting it, you can delete the ```alive.py``` file if you cloned it.

**Functions:**

Default commands for the bot are the following:
- !wordle
- !wordle today
- !custom (code)
- !create (word)
- !guess (word)
- !game
- !active
- !position
- !correct
- !incorrect
- !giveup
- !end
- !help
- !info

Use !help to view the list of commands as well as to see what function each command has. To change the prefix of the bot, replace '!' with 'yourprefix' using the find all, replace feature avaliable to most IDE's.
If you try and play a game on a two different servers, the games will carry across due to the game setup system that was scripted in. Multiple people can start their own games without interference with the use of the ```activegames``` dictionary.

**Notes for customization:**

DO NOT EDIT THE ```emojiID``` DICTIONARY!!<br/>
This dictionary is how the bot prints out custom emojis from several servers I used. To print out an emoji with a Discord bot, you have to use 
```<:emojiname:emojiid>``` which means that everytime I print out an emoji, I need to find the emoji ID as well which is why I put all the ID's into a dictionary.

```activegames``` contains all game info of the player ID that has an active game.
```
activegames[playerID] = {
  'games': 'the board that saves player guesses',
  'guessed': 'last player guess',
  'secretword': 'the word the player is trying to guess',
  'position': 'the correctly positioned letters',
  'correct': 'the correct letters',
  'incorrect': 'the incorrect letters',
  'turn': 'the current turn'
}
```

Invite link: https://discord.com/oauth2/authorize?scope=bot&client_id=956668131110162472 (Official bot) <br/>
![Screen Shot 2022-03-29 at 10 29 56 AM](https://user-images.githubusercontent.com/100868154/160671053-23b5de1c-4978-4cc7-91a2-234204b34436.png)<br/>
![Screen Shot 2022-03-29 at 10 29 19 AM](https://user-images.githubusercontent.com/100868154/160671061-8eca1fff-abf9-4745-bbb2-8ffa19571165.png)<br/>
![Screen Shot 2022-03-29 at 10 30 05 AM](https://user-images.githubusercontent.com/100868154/160671040-e6a83f49-4424-4693-b803-fdd32eaa185e.png)<br/>
