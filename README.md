# Lab - Class 04: Classes and Fixtures

### Author: Ashley Casimir

- [Pull Request URL]() 

### Set it up

Use the following commands to set up the project in the directory of your choosing:

```
$ poetry new pythonic-garage-band
$ cd pythonic-garage-band
$ poetry add --dev black --allow-prereleases
$ touch pythonic_garage_band/band.py
$ touch tests/test_band.py
$ mv README.rst README.md
$ git init
$ git add .
$ git commit -m "first commit"
$ git branch -M main
$ git remote add origin $YOUR_GITHUB_REPO_LINK
$ git push -u origin main
```
Now you are ready to rock and roll!

To start your enviornment use:
- ```$ poetry shell```

To run the program and see the output run:
- `$ python band.py` or `$ python3 band.py` depending on your system


## Feature Tasks and Requirements

Use Python classes to model a `Band` made up of different kinds of musicians.

Start with `Guitarist`,`Bassist`, and `Drummer`.

Make use of a `Musician` base class to handle common functionality which particular kinds of musicians will inherit.

### User Acceptance Tests

Unit tests will be supplied for this lab. Your job is to make them pass. Do NOT modify the supplied tests (except to enable for stretch goals.)

**Band Tests**

- A Band instance should have a name attribute which is a string.

- A Band instance should have a members attribute which is a list of instances that inherit from Musician base (or super) class.

- A Band instance should have a play_solos method that asks each member musician to play a solo, in the order they were added to band.

- A Band instance should have appropriate __str__ and __repr__ methods.

- A Band should have a class method to_list which returns a list of previously created Band instances

**Musician Subclass Tests**

- Each kind of Musician instance should have appropriate __str__ and __repr__ methods.

- Each kind of Musician instance should have a get_instrument method that returns string.

- Each kind of Musician instance should have a play_solo method that returns string.

**Stretch Goals**

- See tests marked “stretch” in supplied test suite.

- Make Musician “abstract” - aka an Abstract Base Class

- Add your own tests.