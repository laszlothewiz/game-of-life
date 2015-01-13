# game-of-life
A game of life implementation based on the Jan 2015 Golang Indy meeting 

This is a sample Go program that works in conjuction
with http://byo-game-of-life.herokuapp.com/ as a back-end.
This example was used in the Indy Golang meetup of Jan 6, 2015.
Rewritten by Laszlo Szenes from Larry Price's example given during the meetup .

The code is mean to be a good example for a simple HTTP API implementation and the use of data types in go.
It contains ample comments to explain every component in the code.

If you find a typo, have a better, more elegant way of implementing Game of Life then submit a pull request.

## How to Use

* Simply compile do a `go run` or `go build` and run the backend. You can change the port number in the code as necessary.
* Go to http://byo-game-of-life.herokuapp.com/ and type in `http://localhost:8080` in the URL box.
* Add some live cells to the board and press either `play` or `step` to see what happens.

## Some interesting initial cell formations

The long lived one. This formation goes through over 1,000 generations of growth before it becomes stagnant
````
##
 ##
 #
````

Fancy oscillation: 
if you place exactly ten cells in a row then it goes through a 15 stage repeating cycle.

The roamer. This formation moves in a diagonal direction, depending on the initial configuation (you can rotate it)
````
##
# #
#
````
The above configuration formation moves up and to the left 
