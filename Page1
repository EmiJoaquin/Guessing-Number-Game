import random
game_over = False
attempts = 0
def index():
  print("Welcome to the Number Guessing Game!")
  print("I'm thinking a number between 1 and 100.")
  mode = input("Choose the dificulty. Type 'e' to easy mode or 'h' to hard mode.").lower()
  global attempts
  if mode == "e":
    attempts += 10
    print("You have {} attempts.".format(attempts))
  elif mode == "h":
    attempts += 5
    print("You have {} attempts.".format(attempts))
  else:
    print("You have to type 'e' or 'h'. Try again.")
    index()
index()

NUMBER = random.randint(1, 100)
print(NUMBER)

def guess():
  guess = int(input("Make a guess:"))
  return guess

def game():
  global attempts
  global game_over
  
  while game_over == False:
    if attempts == 0:
      game_over = True
      print("Game Over!")
    if attempts > 0:
      x = guess()
      if x > NUMBER:
        attempts -= 1
        print("Too high.")
        game()
      elif x < NUMBER:
        attempts -= 1
        print("Too low.")
        game()
      else:
        print("You win")
        game_over = True
game()
