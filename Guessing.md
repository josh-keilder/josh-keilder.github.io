```mermaid
flowchart TD
  Start([Welcome to the Guessing game!]) --> Begin["The game will now begin"]
  Begin --> RandomNumber[Generating a  Random number]
  RandomNumber --> Input["The user may guess a number!"]

  subgraph Guessing
  Input --> IsNumber{Is the input a number?}
    IsNumber -- Yes --> CheckCorrect{Is the number correct?}
    IsNumber -- No --> Error[Input must be a number!] --> Input
    CheckCorrect -- Too High --> HighNumber[Your number is too high!] --> Input
    CheckCorrect -- Too Low --> LowNumber[Your number is too low!] --> Input
    CheckCorrect -- CorrectNumber --> Win["You Win!"]
  Win --> End[The game will now end. Thanks for playing]
```














































