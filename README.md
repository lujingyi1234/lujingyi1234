- 👋 Hi, I’m @lujingyi1234
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
lujingyi1234/lujingyi1234 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
import random

class GuessTheNumber:
    def __init__(self):
        self.target_number = random.randint(1, 100)
        self.attempts = 0

    def play_game(self):
        while True:
            guess = int(input(""))
            self.attempts += 1
            if guess == self.target_number:
                print(f"{self.attempts}")
                break
            elif guess < self.target_number:
                print("")
            else:
                print("")
game = GuessTheNumber()
game.play_game()
