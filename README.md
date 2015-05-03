# DataStructure230

1> Implement the dictionary ADT of Section 4.4 pg. 134, 137 by means of a hash table with linear probing for collision resolution, see proj. 9c6 pg. 349.

2> Implement the test the 2-3+ tree. (Project 10.2 page 378. )

3> Use sfold function on Ex. 9.8 page 329 and the ELFhash function below to solve a, c on problem 9.17 pg. 348 (use code given here with M = 101)

Int Elfhash (Char* key)
{
Unsigned long h - 0;
  while(*key)
  {
  h - (H << 4) + *key++;
  unsigned long g = h & 0xF00000000L;
  if(g) h^ = g >> 24;
  h & ~g;
  }
  return H % M;
  }
