Silver, David, Huang, Aja, Maddison, Chris J., Guez, Arthur,
Sifre, Laurent, van den Driessche, George, Schrittwieser,
Julian, Antonoglou, Ioannis, Panneershelvam, Veda, Lanctot,
Marc, Dieleman, Sander, Grewe, Dominik, Nham, John,
Kalchbrenner, Nal, Sutskever, Ilya, Lillicrap, Timothy, Leach,
Madeleine, Kavukcuoglu, Koray, Graepel, Thore, and Hassabis,
Demis. Mastering the game of go with deep neural networks
and tree search. Nature, 529(7587):484–489, Jan 2016.
Article.

## Goals

Develop an effective (1) move selection and (2) position evaluation functions for Go. And compared to Deep Blue chess engine, aim to (1) evaluate much fewer positions and (2) generate neural networks-based evaluation function which don't need to be handcrafted and can be trained through general-purpose supervised and reinforcement learning methods.

## Summary

AlphaGo achieved a 99.8% winning rate against other Go programs, and defeated the human European Go champion by 5 games to 0, and the Elo rating of non-distributed AlphaGo was ~2890, which is as good as that of the best human player.

AlphaGo uses value networks to evaluate positions and policy networks to sample actions. Although I didn't quite understand the details, they seem to be derived from convolutional neural networks used in image recognition; the board position is passed as a 19 x 19 image, and the output is used to make the search tree small for faster evaluation/sampling.
