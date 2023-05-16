# Alternative Dollar Auction Game: Modeling and Simulation Based on "Thirty-Six Stratagems" and Game Theory.
## Project information
- **Author**: Yiwei Liang, Computation and Design with tracks in Computer Science, Class of 2025, Duke Kunshan University
- **Instructor**: Prof. Luyao Zhang, Duke Kunshan University
- **Disclaimer**: Submissions to the Problem Set No. or Final Project for [COMPSCI/ECON 206 Computational Microeconomics, 2023 Spring (Seven Week - Second)](https://ce.pubpub.org/) instructed by Prof. Luyao Zhang at Duke Kunshan University.
### **Project Summary**: 
  -  Dollar Auction game is a non-zero-sum sequential game played by two or more bidders, with the objective of winning a dollar bill. In this project, develop a new tool to simulate the dollar auction game and change the original game into an alternative form. Consider the real-world application of Dollar Auction game, it usually explains the effects and consequences of sunk costs and costly competition. Applying this project, we have a more flexible Dollar Auction game environment to simulate more complex situations. At the same time, this project provides new solutions to decrease the probability and amount of lost money. 
#### Research Question: What are the effects of incorporating strategies from the "Thirty-Six Stratagems" and game theory in an alternative dollar auction game and how to consider a more complex situation compared to the original dollar auction game.
#### Methodology
The code implements a game that involves two players (`Player1` and `Player2`) competing against each other. The game progresses through multiple rounds, and the players make decisions regarding their moves, strategies, and payments. Here is an overview of the methodology:
##### **Class Definitions**:
- `Content`: Represents the content of the game, including the goods available.
- `Player1`: Represents Player 1 and contains attributes and methods related to Player 1's moves, strategies, and decisions.
- `Player2`: Represents Player 2 and contains attributes and methods related to Player 2's moves, strategies, and decisions.
- `Game`: Represents the game itself and coordinates the interactions between Player 1 and Player 2.
##### Game Flow:
1. The game starts with the creation of Player 1 and Player 2 instances, along with the initialization of game-related variables.
2. Each round of the game consists of the following steps:
   - Player 1 and Player 2 make their moves by calling the `player_move` method.
   - If the players are AI-controlled, a random strategy is chosen. Otherwise, the human player is prompted for their actions.
   - Players decide whether to use stratagems or not. If they choose to use stratagems, they select a specific stratagem and execute it using the `which_stra` method.
   - Players determine their actual pay values for goods and the tell values they want to convey to the opponent.
   - The game handles dependent moves, adjusting pay values based on opponent's tell values and a random factor.
   - Money and goods are updated based on the pay values and a decrease rate.
   - The game determines the winner based on the players' money. The winning player is recorded, along with the winning strategies used.
3. The game continues for multiple rounds until completion.
4. The game keeps track of the real winning results by comparing each player's money to their initial money.
5. The game ends, and the final results are available, including the winner, winning strategies, and real winning statistics.

- **Additional Feature**:

- The game allows for human player interaction, where the human player can make decisions and input pay values for goods when using strategies that depend on opponent's tell values.

This methodology provides an overview of the game's structure, the player interactions, and the progression of rounds. It outlines the key steps involved in each round and how the winner is determined based on player decisions and pay values.
  ### Results:
- Paying a higher value increases the probability of winning the game: The code suggests that players who pay a higher value for goods have a higher chance of winning. This implies that investing more money in goods can potentially lead to a favorable outcome. However, it's important to note that paying a higher value also carries a higher risk of losing value. Players need to find a balance between paying enough to increase their winning probability and avoiding excessive losses.
- Splitting action goods can lead to a more complex situation and reduce damage from irrational opponent options: The code indicates that players have the option to split their actions among different goods. This strategy can make the game more intricate by introducing multiple variables for opponents to consider. It can also serve as a defensive measure against opponents' unpredictable moves, minimizing the impact of their irrational decisions. By diversifying their actions, players can increase their chances of success and mitigate potential losses.
  ### [Intellectual Merits and Practical impacts of your project.]
  
   
Note: please insert the screenshot of the answers to your research question by ChatGPT. The methodology that you use to address the research questions must be more innovative than both the current literature and ChatGPT. 

## Table of Contents

- model
- code
- spotlight
- more about the author
- references

### Model
- Game Environment
- Solution Concept
- Evaluations: e.g. efficiency and fairness

### Code
- Game Environment
- Strategic plays
- Equilibruim Evaluations: e.g. belief, strategy, and payoffs
- oTree Experimental Code 


### Spotlight
- Posters
- Figures
- Slides
- Presentations
- Review articles
- Media appearance

### More about the Author
- headshot
- self-introduction
- Final reflections 
  - intellectual growth
  - professional growth
  - living a purposeful life

### References

- Literature References in [Chicago Author-Date](https://www.chicagomanualofstyle.org/tools_citationguide/citation-guide-2.html) Style and [BibTex](https://scholar.google.com/) 

Levin, Dan, and Luyao Zhang. 2020. “Bridging Level-K to Nash Equilibrium.” *The Review of Economics and Statistics* 104 (6): 1329–40. https://doi.org/10.1162/rest_a_00990.

```
@article{levin2022bridging,
  title={Bridging level-k to nash equilibrium},
  author={Levin, Dan and Zhang, Luyao},
  journal={Review of Economics and Statistics},
  volume={104},
  number={6},
  pages={1329--1340},
  year={2022},
  publisher={MIT Press One Rogers Street, Cambridge, MA 02142-1209, USA journals-info~…}
}
```

