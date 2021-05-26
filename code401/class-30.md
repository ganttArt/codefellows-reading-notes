# Hash Tables

Hashtables are a data structure that utilize key value pairs. This means every Node or Bucket has both a key, and a value. A hashtable traditionally is created from an array.

**Collisions** - What would happen if two different keys resolved to be the same index of the array? This is called a collision. The hash map needs to be able to handle two keys resolving to the same index.

**Bucket Sizes** - Hash Maps can have any number of buckets. If a hash map has only a few buckets it will be densely full and have many collisions. If a hash map has more buckets it will be more sparsely populated, there will be less collisions, but there may be a lot of extra empty space.

**Chaining** - To avoid collisions, you can create links (linked list) to hashes that already have values stored at them.

## Internal Methods

- Add()
  - When adding a new key/value pair to a hashtable:
    - send the key to the GetHash method.
    - Once you determine the index of where it should be placed, go to that index
    - Check if something exists at that index already, if it doesn’t, add it with the key/value pair.
    - If something does exist, add the new key/value pair to the data structure within that bucket.
- Find()
  - The Find takes in a key, gets the Hash, and goes to the index location specified. Once at the index location is found in the array, it is then the responsibility of the algorithm the iterate through the bucket and see if the key exists and return the value.
- Contains()
  - The Contains method will accept a key, and return a bool on if that key exists inside the hashtable. The best way to do this is to have the contains call the GetHash and check the hashtable if the key exists in the table given the index returned.
- GetHash()
  - The GetHash will accept a key as a string, conduct the hash, and then return the index of the array where the key/value should be placed.

## Resources

- Read [Intro to Hash Tables](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-30/resources/Hashtables.html)
- Watch [what is a hash table?](https://www.youtube.com/watch?v=MfhjkfocRR0)
- Read [basics of hash tables](https://www.hackerearth.com/practice/data-structures/hash-tables/basics-of-hash-tables/tutorial/)
- Skim [hash table wiki](https://en.wikipedia.org/wiki/Hash_table)
