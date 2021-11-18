# Coderitter Typescript coding style

**camelcase** : 
- every veriable, constant, class and method should be represented in camelcase
- classes should thereby begin with a capital letter **ClassName**
- attributes, methods, functions, variables and constants should beginn with a lower case letter **methodName**, **functionName**, **variableName**, **constantName**
- **reason** : just uniform style of naming

**semicolons** :
- should never be set in critial cases (for example the next line begins with a bracket)

	`line = line + of + code`
- but: 

	```
      let a = {}
      ;(a as User).name = 'Name'
- **reason**: less charakter in code --> less characters you can forget 

**stroustrup** :
- is the following brace-style:
	```
    if {
        //some code here
    }
    else {
        //some other code here
    }
- **reason** : compromise between 1TBS (else on line from closing-if brace) and Allman (newlin for every brace and if/ else

**mandatory braces**:
- also in controlstatements with only a single line of code there should be braces
	```
   if {
       return true
   }
- **reason** : if you want to change a single line to a multi line if you could forget to set the braces

**indent** :
- 4 spaces
- **reason** : uniform style of indent

**no console** :
- in your pushed code should be no console statement active
- **reason** : we have the lib "knight-log" where statements can be visualized. This logs can be turned on and off, so everyone can see exactly the logs he/ she wanted to see and don't have to search for unwanted disturbing logs, which fill up the hole console.
