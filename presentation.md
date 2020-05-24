Slide 1
Hello my name is Pavel Yermakov. Subject of my presentation Lodash.
What is Lodash?
Slide 2
Lodash is a JavaScript library which provides utility functions for common programming tasks using the functional programming paradigm.
Original author is John-David Dalton.
Initial release:    April 23, 2012. 
Stable release:   July 17, 2019 (v4.17.15). 
NPM Downloads:       (about)~50M / month
NPM Dependends:     >50K
GitHub Stats:               ~280 contributors, ~8K commits, ~40K stars 

Slide 3
Ladash Pros & Cons.
Pros:
Consistency across all major browsers irrespective of their version
Chrome 54+ ,    Firefox 49+,     IE 11,      Edge 14+,      Safari 9+,      Node.js 6+
Allows build semantic data flows.
Facilitates writing pure simple functions.
Documentation is nice and concise.
Easy to start with.
Cons:
Most of errors are silently suppressed and you just get some unobvious value like empty array or object or undefined.
One more external dependency.
Lacks for lazy evaluations.

Slide 4

Main Function Categories
Array
Collection
          Arrays, objects,  and strings
Function
Math
Number
Object
Seq
              Metod chain sequences
String

Slide 5
Main Function Families
is*              checks if value is something;
stub*         returns some predefined value;
to*              converts value into something;
*By               accepts iterate function to generate some extra criterion;
*In                work with both own and inherited properties;
*Deep         recursively works with nested data structures;
*Depth        recursively work with nested data structures up to specified depth;
*Right         performs an operation in reverse order;
*With         accepts comparator, customizer or iterate function to modify make                      algorithm more generic;
*While        accepts function and proceeds only until it returns falsey.


I will tell about some in more detail.

Slide 6
_.isNull(value)
Checks if value is null.
Arguments
value (*): The value to check.
Returns
(boolean): Returns true if value is null, else false.




Slide 7
_.isNumber(value)
Checks if value is classified as a Number primitive or object.

Note: To exclude Infinity, -Infinity, and NaN, which are classified as numbers, use the _.isFinite method.

Arguments
value (*): The value to check.
Returns
     (boolean): Returns true if value is a number, else false.

Slide 8
_.toArray
Converts value to an array.
Arguments
value (*): The value to convert.
Returns
(Array): Returns the converted array.



Slide 9
_.toString
Converts value to a string. An empty string is returned for null and undefined values. The sign of -0 is preserved.
Arguments
value (*): The value to convert.
Returns
(string): Returns the converted string.

Slide 10
_.get
Gets the value at path of object. If the resolved value is undefined, the defaultValue is returned in its place.
Arguments
object (Object): The object to query.
path (Array|string): The path of the property to get.
[defaultValue] (*): The value returned for undefined resolved values.
Returns
(*): Returns the resolved value.
Slide 11
_.groupBy
Creates an object composed of keys generated from the results of running each element of collection thru iteratee. The order of grouped values is determined by the order they occur in collection. The corresponding value of each key is an array of elements responsible for generating the key. The iteratee is invoked with one argument: (value).
Arguments
collection (Array|Object): The collection to iterate over.
[iteratee=_.identity] (Function): The iteratee to transform keys.
Returns
(Object): Returns the composed aggregate object.
Slide 12
_.intersection([arrays])
Creates an array of unique values that are included in all given arrays using SameValueZero for equality comparisons. The order and references of result values are determined by the first array.
Arguments
[arrays] (...Array): The arrays to inspect.
Returns
(Array): Returns the new array of intersecting values.
Slide 13
_.orderBy
This method is like _.sortBy except that it allows specifying the sort orders of the iteratees to sort by. If orders is unspecified, all values are sorted in ascending order. Otherwise, specify an order of "desc" for descending or "asc" for ascending sort order of corresponding values.
Arguments
collection (Array|Object): The collection to iterate over.
[iteratees=[_.identity]] (Array[]|Function[]|Object[]|string[]): The iteratees to sort by.
[orders] (string[]): The sort orders of iteratees.
Returns
(Array): Returns the new sorted array.
Slide 14
_.filter
Iterates over elements of collection, returning an array of all elements predicate returns truthy for. The predicate is invoked with three arguments: (value, index|key, collection).



Arguments
collection (Array|Object): The collection to iterate over.
[predicate=_.identity] (Function): The function invoked per iteration.
Returns
(Array): Returns the new filtered array.

Slide 15
_.find
Iterates over elements of collection, returning the first element predicate returns truthy for. The predicate is invoked with three arguments: (value, index|key, collection).
Arguments
collection (Array|Object): The collection to inspect.
[predicate=_.identity] (Function): The function invoked per iteration.
[fromIndex=0] (number): The index to search from.
Returns
(*): Returns the matched element, else undefined.

Slide 16

For more information on the functionality of Lodash, please visit lodash.com
 
Slide 17

Thank you for your attention











