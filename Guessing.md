# Random Number Guessing Game Flowchart

**This flowchart models a number guessing game. The computer selects a random number and the user keeps guessing numbers until they find the correct one.** 

If they do not enter a valid input, it will prompt the user for another guess. If the guess is incorrect, the computer will notify and help the user by telling them if their guess was too high or too low. It will them reprompt the user to try again until the user finally guesses correctly. The gaame ends when this happens and it will notify the user that they were correct.


```mermaid
flowchart TD
    A[Start] --> B[Generate Random Number]
    B --> C[Prompt User for a Guess]
    C --> D{Is Input Valid?}
    D -- No --> E[Display 'Invalid Input'] --> C
    D -- Yes --> F{Is Guess Correct?}
    F -- Yes --> G[Display 'Correct!'] --> H[End]
    F -- No --> I{Is Guess Too High?}
    I -- Yes --> J[Display 'Too High'] --> C
    I -- No --> K[Display 'Too Low'] --> C
```
