---
title: Self Hosting
weight: -15
---

To host the bot yourself, follow these simple instructions.

<!--more-->

- Download the bot from [this](https://github.com/vrnavi/dishwasher) repository. Stick to the release versions unless you have encountered a bug.
- Install [pipenv](https://pipenv.pypa.io/en/latest/).
- Use `pipenv install` in the root folder, where `Pipfile` is.
- Copy `config.example.py` to `config.py`, and fill it out with your bot information.
- Enter `pipenv shell`, `cd dishwasher`, then `python __init__.py`.
- Congratulations.

I will not help you if you wish to use a `requirements.txt`.
