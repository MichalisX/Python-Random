# Creating a deck of cards
import random
import itertools

suits = ['spades', 'hearts', 'clubs', 'diamonds']
vals = ['Ace', '2', '3', '4', '5', '6', '7', '8', '9', 'T', 'J', 'Q', 'K']

deck = list (itertools.product(vals, suits))

random.shuffle(deck)

for vals, suits in deck:
    print ('The %s of %s' % (vals, suits))
