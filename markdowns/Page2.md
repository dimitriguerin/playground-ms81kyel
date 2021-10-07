<script>
let randomNumber = Math.floor(Math.random() * 100) + 1;

let guesses = document.querySelector('.guesses');
let lastResult = document.querySelector('.lastResult');
let lowOrHi = document.querySelector('.lowOrHi');

let guessSubmit = document.querySelector('.guessSubmit');
let guessField = document.querySelector('.guessField');

let guessCount = 1;
let resetButton;
  
  <p class="guesses"></p>
<p class="lastResult"></p>
<p class="lowOrHi"></p>
  
  <label for="guessField">Enter a guess: </label><input type="text" id="guessField" class="guessField">
<input type="submit" value="Submit guess" class="guessSubmit">
  
  function checkGuess() {
  alert('Je suis un espace réservé');
}
  
  checkGuess();
  
  let name = 'Bingo';
name;
let hello = ' dit bonjour !';
hello;
let greeting = name + hello;
greeting;
  
  name += ' dit bonjour !';
  name = name + ' dit bonjour !';
  
  function checkGuess(){
  let userGuess = Number(guessField.value);
  if (guessCount === 1) {
    guesses.textContent = 'Propositions précédentes : ';
  }
  guesses.textContent += userGuess + ' ';

  if (userGuess === randomNumber) {
    lastResult.textContent = 'Bravo, vous avez trouvé le nombre !';
    lastResult.style.backgroundColor = 'green';
    lowOrHi.textContent = '';
    setGameOver();
  } else if (guessCount === 10) {
     lastResult.textContent = '!!! PERDU !!!';
     setGameOver();
  } else {
     lastResult.textContent = 'Faux !';
     lastResult.style.backgroundColor = 'red';
     if (userGuess < randomNumber) {
      lowOrHi.textContent = 'Le nombre saisi est trop petit !';
     } else if (userGuess > randomNumber) {
      lowOrHi.textContent = 'Le nombre saisi est trop grand !';
     }
  }

  guessCount++;
  guessField.value = '';
  guessField.focus();
}

  guessCount === 1
  guessSubmit.addEventListener('click', checkGuess);
  function setGameOver() {
  guessField.disabled = true;
  guessSubmit.disabled = true;
  resetButton = document.createElement('button');
  resetButton.textContent = 'Start new game';
  document.body.appendChild(resetButton);
  resetButton.addEventListener('click', resetGame);
}
  
  function resetGame() {
  guessCount = 1;

  let resetParas = document.querySelectorAll('.resultParas p');
  for (let i = 0 ; i < resetParas.length ; i++) {
    resetParas[i].textContent = '';
  }

  resetButton.parentNode.removeChild(resetButton);

  guessField.disabled = false;
  guessSubmit.disabled = false;
  guessField.value = '';
  guessField.focus();

  lastResult.style.backgroundColor = 'white';

  randomNumber = Math.floor(Math.random() * 100) + 1;
}
                                        for (let i = 1 ; i < 21 ; i++) { console.log(i) }
  
  let resetParas = document.querySelectorAll('.resultParas p');
for (let i = 0 ; i < resetParas.length ; i++) {
  resetParas[i].textContent = '';
}
                                      guessField.focus();
                                      
                                      let guessField = document.querySelector('.guessField');
                                      guessField.focus();
                                      guessField.value = 'Hello';
guesses.value
guesses.textContent = 'Where is my paragraph?';
guesses.style.backgroundColor = 'yellow';
guesses.style.fontSize = '200%';
guesses.style.padding = '10px';
guesses.style.boxShadow = '3px 3px 6px black';
                                      
</script>
