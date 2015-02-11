##Descriptions of Iterators

###Instructions
Below you will find a list of methods. In the space provided below each, please provide a brief description of what this method does based upon your review of the Docs. 

###Array methods:
May be helpful to look in [Enumerable](http://ruby-doc.org/core-2.2.0/Enumerable.html) as well...

####select: The select method returns an array of members of the calling array that pass the test in its block. If there is no test the array is returned.

####reject: Returns an array of the members of the calling array that DID NOT pass the test in the block. If no test was given, it returns the an array.

####map: Runs the code in the block for each member of the calling array and returns an array of the values and if no block of code is given it returns a copy of the calling array.

####detect: Passes each member of the array(or enumerator) to the block and returns the first member to pass the test or returns true. If no member passes it returns the value provided by the ifnone option that comes before the block. If no ifnone value is provided, then it returns nil. If no block is given then it returns the calling array.

####inject: This is like JS reduce iterator. It uses the code in the block or the method represented by the symbol provided. It keeps the result from each iteration and passes it in for the next iteration. !worth reviewing!

####partition: This method returns two arrays, one array has all elements of the calling array that return true from the code in the block and the other is an array of the remaining elements.

####sort: Returns an array in which the calling array's elements are sorted. If passed a block the block has to return a similar result of using <=>. 

####one?: one? returns true if only one of the elements of the calling array (or enumerator) returns true to the code in the block. If no block is given, it only returns true if the calling array only has one "truthy" value.

####none?: Returns true if all the members of the calling array return a false from the array. If no block is given, then it only returns true if all elements in the calling array evealuate to false.

####all?: Passes every element of the calling array returns true or a truthy value when when passed to the code in the block. If no block is given then it uses an implicit block that returns true if each member is not false or nil.

####empty?: Returns true if the calling array contains no members or elements.

####eql?: Returns true if calling array and another array are the same object or if the two are arrays and have identical content. It is an object method.

####include?: Returns true if any member of the calling array is equal to the supplied object i.e. the object is contained in the array.

####nil?: Returns nil if the object is nil.

###Hash methods: 

####key?: Returns true if the key is in the calling-hash

####keys: Returns an array consisting the keys of the calling hash

####delete: Deletes specified key and returns the value associated with it. If the key is not in the hash, it returns the default value. If the optional code is added, and there was no matching key, the key is added to the calling hash and the value of the code is returned.

####delete_if: Deletes every key-value pair that the code returns true to and returns a hash equal to what is left of the calling hash after the deletion. If no code is given, it returns the calling hash
