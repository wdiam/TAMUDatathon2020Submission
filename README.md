# TAMUDatathon 2020 Submission

## Lone Wolf and Cub(s) Stock Prediction

Howdy!

This is the repository (just a notebook, really) tied to the winning submission for the [TAMUDatathon 2020](https://tamudatathon.com/) "Stock Prediction" challenge. Further details, including the provenance of the challenge, can be found at the [formal devpost.com submission](https://devpost.com/software/lone-wolf-and-cub-s-stock-prediction-kiz3w5).

The crux of the challenge is that we have daily mystery stock data, a bunch of covariates, and we want to predict next day's return. The twist is that for a consequent buy/sell, we need to place a "fraction" for how much to stake our capital.

For some more context, this was a competition held for undergraduate students, graduate students, and people who gradudated within a year from when the competition was held. As such, I technically participated while being a master's student in Statistics from Texas A&M. 

## Post Mortem & Caveats

This submission/solution ended up being the winning approach, but there are a litany of reasons why it may not be realistic, including but not limited to liquidity, what's the actual spread, no transaction costs were imposed, etc. Even more so, there's a lot of variance in this whole process that consequently gives you a fighting chance, even with a sub-optimal submission. That being said, imposing and/or correcting for all of "that" would potentially have made the challenge less fun for others and just more things to deal with in a 24 hour period. In any case, **I** had fun tooling around and messing with this.

Also, ***to get the most out of this notebook***, you shouldn't really focus too much on the "stock" aspect and instead think of the following as a template for a supervised learning problem and an example of how one constructs pipelines and related items. Really, the way I treated this, was I'm given "X" and "y", now go build a good predictor and everything else was auxiliary.
