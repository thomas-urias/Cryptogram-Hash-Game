# Cryptogram-Hash-Game
Cryptogram-Hash-Game is a puzzle game where the player tries to decode a scrambled phrase. The phrase has been encrypted using a cryptogram style algorithm, and the player wins once the entire message is correctly decoded. The game includes helpful tools such as letter frequency checks and optional hints to make the puzzle easier to solve.

The game is built using the Model-View-Controller (MVC) structure:

Model: Stores all the game data, including the scrambled phrase, the player’s current guesses, and hint information. The model also checks if the player’s substitutions are correct and whether the phrase is fully solved. It implements Serializable, allowing the game state to be saved and loaded.

View: Displays the game to the player: showing the scrambled phrase, entered letters, hints, and frequency information. It updates whenever the model changes.

Controller: Handles player actions, such as entering letter guesses, checking frequencies, or asking for hints. It passes these actions to the model and tells the view when to update.

Using MVC keeps the game organized and makes the code easier to maintain. Serialization in the model ensures players can save their progress and continue later.
