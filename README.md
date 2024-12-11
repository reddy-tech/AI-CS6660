# AI-CS6660


# X-s-O-s

The submitted file is for the Term Project for the course Introduction to Artificial Intelligence Fall 2024.The group members for this project are Yashwanth and Srenitha.

A X-s-O-s game is developed using different artificial intelligence agents. We have implemented the game using the following four agents with their variations: Expectimax, Minimax, Alpha- Beta, Q learning and Approximate Q learning algorithms.

# X’s and O’s Game

A two-player game where players take turns placing X's and O's on a grid defined by two horizontal and two vertical lines, aiming to be the first to align three consecutive X's or O's in a row.

# Objectives

* Implementation of X’s and O’s using multiple agents.
* Playing the game using the designed models.
* Agent forming the quickest sequence and remaining undefeated till the end is declared as our winner.

# Approach

* Designing a layout which is a 3x3 grid.
* Agent training about the game play atmosphere using Expectimax, Minimax, Alpha- Beta, Q learning and Approximate Q learning algorithms.
* Define the agent which minimizes our utility and develop a counter strategy for our self to maximize our utility
* The limitations of minimax can be overcomed by using expectimax which further expands our utility.
* Further, we add a choice node to study actions of the agent and use Q learning algorithm to get the maximum utility.

# Agents Used

### Expectimax Agent
* The Expectimax algorithm, based on game theory, aims to maximize expected utility. It is a modified version of the Minimax algorithm, but unlike Minimax, it does not assume that the adversary (the minimizer) is acting optimally. This makes it useful for scenarios where the opponent’s behavior is unpredictable or random.

* Expectimax is beneficial for taking advantage of less-than-ideal opponents. Since opponents can behave unpredictably, the algorithm is capable of 'taking risks,' which may lead to a higher utility state compared to Minimax, even though it's not necessarily optimal.
  
* In Expectimax, the Chance nodes estimate the expected utility by averaging the utilities of all possible outcomes.
### Minimax Agent
* Minimax is a recursive method used to find the best move for a player, assuming the opponent is also making optimal decisions. The goal, as suggested by its name, is to minimize the maximum possible loss (reduce the worst-case outcome).
  
* The Minimax algorithm works through a sequence of moves between two players, where the player whose turn it is strives to maximize their score. Meanwhile, the opposing player evaluates the potential moves, choosing the one that leads to the lowest possible score for the maximizer.

* This function utilizes minimax() to evaluate all possible moves and then selects the best move for the player aiming to maximize their score.

### Alpha- Beta Agent
* Alpha-beta pruning is a popular enhancement to the basic algorithm that applies a more relaxed criterion to determine when nodes in a tree can be discarded.

* This technique is particularly useful in the Minimax algorithm. As the depth of the game tree increases, the number of game states the Minimax algorithm needs to evaluate grows exponentially.

* Although it's impossible to completely eliminate this exponential growth, it can be reduced significantly.

* The pruning technique allows us to compute the optimal Minimax decision without having to examine every node in the game tree.

* This process uses two parameters, Alpha and Beta, to manage the pruning and is known as alpha-beta pruning.

### Q learning Agent
* In contrast to traditional game theory approaches like the Minimax algorithm, which assumes the opponent is perfectly rational and aims to maximize its own reward while minimizing the agent's, reinforcement learning does not require a model of the opponent, and it can still yield surprisingly effective results.

* When tackling reinforcement learning problems, it is crucial to focus on the three main components: state, action, and reward. First, train two agents to compete against each other, saving their policies after 5000 rounds. Next, have the agent play against humans by loading its learned policy.

* We need a player class that represents our agency and can do the following:
  * Choose actions depending on the current status estimation.
  * Keep track of the game's many states.
  * After each game, update the states-value estimation.
  * The policy should be saved and loaded.


# Requirements:
###### Python 3.7

# Execution Guidelines:
###### Execute the ticTacToe.py file to start the game.
