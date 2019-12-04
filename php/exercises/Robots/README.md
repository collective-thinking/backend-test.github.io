# Robot Name

Manage a robot factory.

The factory produces two types of robots: 
  - Flying robots, that can fly
  - Walking robots, that can walk

When robots come off the factory floor, they have no name.

The first time you boot them up, a random name is generated in the format of :
  - two uppercase letters prefix defining the type of robot
    - FL for flying robots
    - WK for walking robots
  - followed by three digits
  - followed by 2 uppercase letters

Ex: FL837RX or WK811BC...

Every once in a while we need to reset a robot to its factory settings,
which means that their name gets wiped. The next time you ask, it will
respond with a new random name.

The names must be random: they should not follow a predictable sequence.
Random names means a risk of collisions. Your solution must ensure that
every existing robot has a unique name.

**Your solution should make possible:**
 - the making of robots of both types
 - make flying robots fly (a simple `echo` is sufficient)
 - make walking robots walk (a simple `echo` is sufficient)
 - get the name of each robots
 - uniqueness of robots name
 - reset each robots
 
You can create as many files, classes, methods... as you want. (in this folder)
Make your solution as elegant and maintainable as possible, following the **SOLID** principles.

**Bonus:** Add unit tests to your solution.
