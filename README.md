# Role-playing-game
This is a Git repository for a JavaScript-based role-playing game. Explore the code and contribute to the development of this exciting adventure.

## Gameplay
The game is a turn-based battle between the player character and a series of monsters, with the outcome determined by the roll of a virtual dice.
This is a game that involves a player character (a wizard) battling against various monsters. The game mechanics involve using dice to determine damage dealt and taken by both the wizard and the monster. Each monster has its own set of data defined in an external file that is imported into the code.
The attack() function is the main gameplay loop. When the player clicks on the "attack" button, the function is called. You can therefore attack the monster and produce a result. The wizard and monster both roll their dice and deal damage to each other based on the resulting scores. If the wizard's health reaches zero, the game ends with a loss. If the monster's health reaches zero the wizard wins.
## How is made
I created this game using JS ES6, CSS, and HTML. Features include:

- Engaging gameplay mechanics
- Responsive design for optimal performance on desktop and mobile devices
- Constructor function
- Destructuring and Object assignment
- SetTimeout, map, reduce and utils functions.
## Links
Try the online version
https://emazack.github.io/role-playing-game/
## Main functions
- The getNewMonster() function retrieves the next monster from the monstersArray and creates a new Character object using data from the characterData object.
- The attack() function is called whenever the "attack-button" is clicked. It checks whether the game is waiting for a new monster (i.e., the current monster has been defeated), and if not, it sets the dice scores for the wizard and monster, deducts damage from each character's health points, and renders the updated game state.
- The endGame() function sets a waiting period of 1.5 seconds and then displays a message indicating which character has won. The message is stored in the endMessage variable, and an appropriate emoji is selected and stored in the endEmoji variable. The HTML body is then updated with a message div containing the end message and emoji.
- The render() function updates the HTML of the hero and monster character divs with the current state of the hero and monster characters. The initial state is set at the end of the code by creating a new Character object for the hero and retrieving the first monster from the monstersArray. The render() function is then called to display the initial state of the game.

