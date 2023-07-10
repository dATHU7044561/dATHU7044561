
// Generate a random number between 1 and 100
const targetNumber = Math.floor(Math.random() * 100) + 1;

// Function to start the game
function startGame() {
  // Get user's guess
  const userGuess = parseInt(prompt("Guess a number between 1 and 100:"));

  // Check if the guess is correct
  if (userGuess === targetNumber) {
    alert("Congratulations! You guessed the correct number!");
  } else {
    // Provide feedback if the guess is too high or too low
    if (userGuess > targetNumber) {
      alert("Too high! Try again.");
    } else {
      alert("Too low! Try again.");
    }
    // Give the user another chance to guess
    startGame();
  }
}

// Start the game
startGame();
