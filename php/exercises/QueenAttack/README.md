# Queen Attack

Given the position of two queens on a chess board, indicate whether or not they
are positioned so that they can attack each other.

In the game of chess, a queen can attack pieces which are on the same
row, column, or diagonal.

A chessboard can be represented by an 8 by 8 array.

So if you're told the white queen is at (2, 3) and the black queen at
(5, 6), then you'd know you've got a set-up like so:

```text
_ _ _ _ _ _ _ _
_ _ _ _ _ _ _ _
_ _ _ W _ _ _ _
_ _ _ _ _ _ _ _
_ _ _ _ _ _ _ _
_ _ _ _ _ _ B _
_ _ _ _ _ _ _ _
_ _ _ _ _ _ _ _
```

You'd also be able to answer whether the queens can attack each other.
In this case, that answer would be yes, they can, because both pieces
share a diagonal.

-----------

Your task is to implement two methods:

#### `placeQueen(int $i, int $j): bool` 

Returns `true` if the queen's coordinates are valid on the chessboard of 8 by 8.
Throws an `InvalidArgumentException` otherwise.


#### `canAttack(array $white, array $black): bool`

Method arguments are the coordinates of the white and black queens as arrays. (`[2, 3]` and `[5,6]`)

Throws an `InvalidArgumentException` if the coordinates of one of the queens is invalid.

Returns `true` if the queens can attack each other, `false` otherwise

