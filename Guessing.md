flowchart TD
  Start[Welcome to the Guessing game!] --> Begin[The game will now begin]
  Begin --> RandomNumber{Generate Random number]
  RandomNumber --> Input[The user may guess a number]
  Input --> IsNumber{Is the input a number?}
  IsNumber -- Yes --> CheckCorrect{Is the number correct?}
  Isnumber -- No --> Error[Input must be a number!] --> Input
  CheckCorrect -- Too High --> HighNumber[Your number is too high!] --> Input
  CheckCorrect -- Too Low --> LowNumber[Your number is too low!] --> Input
  CheckCorrect -- CorrectNumber --> Win[You Win! --> End[End]















































