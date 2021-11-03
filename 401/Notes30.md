# Hash Tables

Terminology:

1. **Hash** - A hash is the result of some algorithm taking an incoming string and converting it into a value that could be used for either security or some other purpose. In the case of a hashtable, it is used to determine the index of the array.

2. **Buckets** - A bucket is what is contained in each index of the array of the hashtable. Each index is a bucket. An index could potentially contain multiple key/value pairs if a collision occurs.

3. **Collisions** - A collision is what happens when more than one key gets hashed to the same location of the hashtable.

Hashtable is a data structure where data is stored in an array format. Every data value has a unique key value. If the key is known, access to the needed data is very fast. So, insertion and search operations are fast independently on the data size. 

Hash Table consists of an array to keep data and hashing for generation an index where an element should be located.

We can use tjem in many applications, such as:

1. Dictionary

2. Library

## Hashing

It is a rule that maps the Object into a set of characters (code). Usually that kind of function converts a big piece of data into a small integer value.

There are three ways of calculating the hash function:

1. Division method

2. Folding method

3. Mid square method