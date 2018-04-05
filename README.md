# sot-web-101
A super-basic (and not so ugly anymore!) web page to show off the basics for SoT hackfest.

## Viewing the webpage in your browser
We recommend using the simple python server to serve up the webpage locally (You will need python installed https://www.python.org/ (If you have a Mac or a Linux machine you probably already have it installed)).

We need to use the command line to run the python server. [Mac users can use Terminal](http://www.wikihow.com/Open-a-Terminal-Window-in-Mac), [Windows users can use the Command Prompt](http://www.digitalcitizen.life/7-ways-launch-command-prompt-windows-7-windows-8), and Linux users should use whatever terminal app comes with their distro.

In your terminal/command line app navigate to the folder where index.html is located in your cloned repo (If you don't know what to do [Windows users can look here](http://www.digitalcitizen.life/command-prompt-how-use-basic-commands), [Linux and Mac users can look here](http://linuxcommand.org/lc3_lts0020.php)). Then run the command `python -m SimpleHTTPServer 8000`. When that is running you can point your browser to http://localhost:8000 to see the page running.

_Note: SimpleHTTPServer will default to serving the index.html file at the root url_

_Note: If you are using python 3 then I think you will need to run_ `python -m http.server 8000` _instead._

Things to fix up on the page:
* [x] Make the heading say something useful by editing the h1 tag in index.html _(maybe something like 'hello world' yeah?)_
* [x] Make the purple text purple by filling in the definition for the 'purple' css class in index.css _(If you want to learn more [here is a good guide for getting started with css](https://developer.mozilla.org/en-US/docs/Learn/CSS/Introduction_to_CSS). I recommend looking at the [tutorial for css selectors](https://developer.mozilla.org/en-US/docs/Learn/CSS/Introduction_to_CSS/Selectors) as it comes in handy for interacting with the page via javascript)_
* [x] Make the button print "Oh hi!" into the results-area div by binding a javascript function to the click action on the button element _(hint: start with line 11 in index.js.)_
* [x] Do something cool with the fetchRandomTriviaQuestion and displayQuestionAndAnswer functions _(hint: maybe you can combine them and hook them up to the function that is called when the button is clicked?)_
* [x] Add some more information to the page. Write a couple of paragraphs about yourself. Add some stock photos of people riding horses. Add a link to your favourite youtube video... Play around with the html a bit.
* [x] Make the page less ugly. Write some css to make the layout nicer. Use a prettier font for all the text. Change the colours up. Experiment with what you can do.
* [ ] Make the page display the current time (updated every second)
* [ ] Build a number guessing game into the page. Rules:
  * Computer picks random number between 1 and 100
  * Player has 6 lives
  * Player attempts to guess the number
  * Game says 'too high', 'too low', or 'you win!'
  * If the guess is incorrect: player looses a life and they get to guess again
  * When lives run out the game is over
* [ ] Customise the trivia game to be multi-choice instead of true or false (generate a new api url here: https://opentdb.com/api_config.php)
  * Can extend this to allow the player to choose the trivia category before they begin the trivia game
