# Hash Tables

![hashTables](https://www.tutorialspoint.com/data_structures_algorithms/images/hash_function.jpg)

Hatch table is a data structure its basically  an array of a list. Each list is known as a bucket A Hash table contains values based on the key.

we use Hatch tables to:

1. Hold unique values
2. Dictionary
3. Library

## complexity

The time complexity O(1) and the time complexity when searching for a piece of data in a collection is O(N)

## Structure

### Hashing

Its the process of converting a key into integer,the hash is created from an array.

### Collisions

A collision occurs when more than one key hashes to the same index in an array.

## Bucket Sizes

Hash Maps can have any number of buckets. If a hash map has only a few buckets it will be densely full and have many collisions. If a hash map has more buckets it will be more sparsely populated, there will be less collisions, but there may be a lot of extra empty space.

## Internal Methods for Hatch table

* Add()

* Find()

* Contains()

* GetHash()

## Resources used in this reading

1. [Hash tables](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-30/resources/Hashtables.html)
2. [video](https://www.youtube.com/watch?v=MfhjkfocRR0)
3. [Basics of Hash Tables](https://www.hackerearth.com/practice/data-structures/hash-tables/basics-of-hash-tables/tutorial/)
4. [Hash table](https://en.wikipedia.org/wiki/Hash_table)