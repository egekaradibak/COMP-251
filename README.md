# COMP-251-A1
Comp 251 assignments Fall 2020
Building a Hash Table
We want to compare the performance of hash tables implemented using chaining and open addressing. In this assignment, we will consider hash tables implemented using the multiplication and linear probing methods. We will (respectively) call the hash functions h and g and describe them below. Note that we are using the hash function h to define g.
Collisions solved by chaining (multiplication method): h(k) = ((A · k) mod 2w) >> (w − r) Open addressing (linear probing): g(k, i) = (h(k) + i) mod 2r
In the formula above, r and w are two integers such that w > r, and A is a random number such that 2w−1 < A < 2w. In addition, let n be the number of keys inserted, and m the num- ber of slots in the hash tables. Here, we set m = 2r and r = ⌈w/2⌉. The load factor α is equal to mn .
We want to estimate the number of collisions when inserting keys with respect to keys and the choice of values for A.
