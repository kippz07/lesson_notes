# Ruby
---

***puts*** *"text"* - prints the text and adds a new line below

***prints*** *"text"* - prints text but does not print a new line

***.length*** - return the length of a string

***.reverse*** - reverses a string

***.upcase, .downcase*** - change to upper or lower case

***\#*** - make a comment

***=begin, =end*** - start, end a comment section, need to be put on their own lines

***gets*** - gets input from the user

***gets.chomp*** - gets input and removes the extra black line that is automatically added when getting an input

**String interpolation:**   
name = "Jenny"  
puts "My name is \#{name}" - prints "My name is Jenny"

***.capitalize*** - capitalises first letter of a string and makes the rest lower case

***!*** - comes after a method, the value contanied in the variable is modified and it doesnt have to be reassigned

--

***if*** *condition*  
*code to be executed*  - loops must be ended with 'end'  
***end***

***elsif*** - the else if condition

***unless*** - 'unless' checks if something is false

***&&*** - and

***||*** - or

***!*** - not

***?*** - methods that end in ? usually evaluate to true or false

***.include?"x"*** - true is string contains what is in the quotes, false if not

***.gsub!(/x/, "y")*** - global substitution, replace x with y

***while..... do***   - while loops also need an 'end'  
***end***

*i = 0*  
***until*** *i = 6*  - 'until' loops execute the loop until the condition is met  
*i += 1*  
***end***

**No ++ or -- in ruby**

***for*** *num* ***in*** *1...10*  - three dots means final number is excluded  
*puts num*  
***end***

***for*** *num* ***in*** *1..10* - two dots means last number is included

**Curly braces { } are interchangable with do, end**

***loop do***  - simplest loop iterater  
***end***

*i = 20*  
***loop do***  
*1 -= 1*  
*print "#{i}"*  
***break if*** *i < 0*  - 'break' breaks the loop f the condition is met  
***end***

***next*** - used to skip over certain steps in the loop:  
***next if*** *i % 2 == 0* - all even numbers of i are skipped

--

*my_array = [1, 2, 3]* - initialise an array

***.each*** - applies an expression to each element in an object, one at a time

object***.each { |*** *var* ***|*** *do something with var* ***}***

10***.times {*** *print "hello"* ***}*** - .times performs a task on each item in the object a specified number of times

***.split(" ")*** - splits a string where it sees the delimiter and returns an array

--

**Hash - a collection of key-value pairs**

*my_hash* ***= {***  
*key1 => value1*  - assign values using =>  
*key2 => value2*  
***}***

*my_hash[key1]* outputs value1

*my_hash* ***= Hash.new*** - creates a new, empty hash

*my\_hash["new\_key"] = new\_value* - add a new key-value pair to the hash

*numbers****.each{|*** element ***|*** puts element ***}*** - iterates over an array

***.each do |****subarray****|***  - iterate over multidimensional arrays  
*subarray****.each { |*** item ***|*** *puts item*  
***end***

hash***.each { |*** *key, value* ***| }*** - hash needs 2 placeholder variables to iterate over

***Hash.new***("x") - give a default value for the hash

