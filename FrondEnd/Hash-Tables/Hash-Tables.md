## Hashtables


### What is a Hashtable?

1. Hash - A hash is the result of some algorithm taking an incoming string and converting it into a value that could be used for either security or some other purpose. In the case of a hashtable, it is used to determine the index of the array.

2. Buckets - A bucket is what is contained in each index of the array of the hashtable. Each index is a bucket. An index could potentially contain multiple key/value pairs if a collision occurs.


3. Collisions - A collision is what happens when more than one key gets hashed to the same location of the hashtable.

### Why do we use them?

1. Hold unique values
2. Dictionary
3. Library

### What Are they?

Hashtables are a data structure that utilize key value pairs. This means every Node or Bucket has both a key, and a value.

exapmple:

```
["Greenwood:98103", "Downtown:98101", "Alki Beach:98116", "Bainbridge Island:98110", ...]
```

### Structure

**Hashing**: Basically, a hash code turns a key into an integer.

**Creating a Hash** :

1. Add or multiply all the ASCII values together.
2. Multiply it by a prime number such as 599.
3. Use modulo to get the remainder of the result, 
 when divided by the total size of the array.
5. Insert into the array at that index.


Example: 
```
Key = "Cat"
Value = "Josie"

67 + 97 + 116 = 280

280 * 599 = 69648

69648 % 1024 = 16

Key gets placed in index of 16. 

```
**Collisions**


A collision occurs when more than one key hashes to the same index in an array. As mentioned earlier, a “perfect hash” will never have any collisions. To put this into perspective, the worst possible hash is one that hashes every single key to the same exact index of an array. The more keys you have hashed to a specific index, the more key/value pair combos you can potentially have.


### Hash Code Examples

```
SUM HASHED: Pioneer Square = 1379
SUM HASHED: Alki Beach = 884
SUM HASHED: U District = 955

BUCKET SIZE=99
SUM INDEX: 1379 % 99 = 92
SUM INDEX:  884 % 99 = 92
SUM INDEX:  995 % 99 = 64

```
