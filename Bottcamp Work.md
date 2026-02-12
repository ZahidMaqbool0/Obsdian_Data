# Bootcamp-Daily-Task-Record
🚀 Daily Bootcamp progress — Learning, Coding, and Growing every day.

# Day 1 - Wednesday - 1 : October : 2025
# Day 2 - Thursday - 2 : October : 2025
# Day 3 - Friday - 3 : October : 2025
# Day 4 - Saturday - 4 : October : 2025
# Day 5 - Sunday - 5 : October : 2025
---
# JOINING START BOOTCAMP
---
# Day 6 - Monday - 6 : October : 2025
1. Obsidian install, and way we use.
2. Cover Markdown language and format.
3. Obsidian custom and Community plugin explore
4. Explore calendar community plugin
5. Create a one project weekly task management plan 
6. Git and GitHub Basic Cover
# Day 7 - Tuesday - 7 : October : 2025
1. Git and GitHub Explore and command cover
2. Git and GitHub commands learn and perform practical examples
3. On GitHub one  project uplod using CMD command
4. Explore the GitHub Desktop
5. Explore GitHub in obsidian
6. Connect GitHub obsidian and uplod daily task 
7. Perform Git, GitHub, Obsidian Git practical example 
# Day 8 - Wednesday - 8 : October : 2025
1. Practice Obsidian Git (Create a new obsidian vault and connect GitHub, and perform git settings automatic)
2. Dart Overview (Introduction)
	- Dart setup
	- Why we use void main function in dart
	- Why we use void in dart language
	- Literals, Variables and Data Types (`int`, `double`, `String`, `bool`) and Types of Variables (`var`, `final`, `const`, `dynamic`, `late`)
	- Understanding Dynamic and Var
	- Understanding final and const
	- Difference between const and final, dynamic and var 
	- Dart Operators Additive (`+`,`-`), Mathematical (`Basic Math` `operator` `*, /, %, ~/`), Assignment (`=, +=, -=, *=, /=, ~/=`), Unary & Relational (`<, >, >=, <=`)
	- Strings Explained: Single-Line, Multiline, escape characters & Interpolation
	- How to index works in string
	- Conditional Statements in Dart: if, else, else if & Ternary Operator
	- Loops in Dart: For, While, and Do-While
	- Lists, Set, Map in Dart
# Day 9 - Thursday - 9 : October : 2025
1. Functions in Dart: Nested, Arrow Functions, and Parameter Types 
	> **Types of parameter** 
	1. Required parameter / positional parameter 
    2. Optional positional parameter `[]`
	3. Optional named parameter `{}` 
    4. Default value parameter
    5. Named Required Parameter
2. Function Data Type, Higher-Order Functions, and Anonymous
3. Break and Continue keyword
4. Practice List
	- **List Practice Question**
	1. Create a list of 5 fruit names and print them.
    2. Store 5 numbers in a list and print the sum of all numbers.
		- Print using for Each Loop
		- print using For In Loop
    3. Update one element in the list (e.g., change the value at index 2).
	4. Remove duplicate values from a list.
# Day 10 - Friday - 10 : October : 2025
1. What is State.
2. What is State Management
3. 3 main ways to manage state in Flutter mean (**State Management main 3 types** )
	- Local State => (`setState()`)
	- App State => (`Bloc`, `Redux`)
	- Shared State (`Provider`, `Riverpod`, `Bloc`)
4. **Types of Widgets:**
	- **Stateless Widget** → UI fix hoti hai (no data change)
	- **Stateful Widget** → UI data change hoti hai (setState use hota hai)
5. Stateful Widget Lifecycle and Stateless Widgets Lifecycle
6. StatefulBuilder (same as it work as setState(),  but it is use in one widgets.)
7. # Null Safety (`?` , `!`, `??` )
	- **Nullable (`?`)** Variable me `null` value allow hoti hai. as ko DataType ka sath lihty ha.
	- **Null Assertion (`!`)** jab hum ko confirm huu ka variable null nahi ho ga.
	- **Null-aware Operator (`?.`)** agr value null mill jati ha tu crash nahi ho gi application balky null return karda gi. agr hum Null aware operator use kara ha. **Example** user?.name;  // If user == null → returns null (no crash)
	- **Null-coalescing Operator (`??`)** as ma hum defulat value set karta ha agr as ko varible ki value null mill jati ha tu ya defult value set kardata ha
	- **late keyword** as ma hum varible ko declear karta waqt yaqeen dalwaty ha ka hum as ko zaror valu assign kara ga ya value zaror ay gi..
8. num keyword (num Data Type) (combination of int and double) 
---
# Day 11 - Saturday - 11 : October : 2025
1. Exception Handling
	- `try`, `catch`, => jab hum ko expection ka na pata huu
	- `try` `on` => jab hum ko pata huu ka kon sa error a sakt ha.
	- `try` `catch` `finally` => ya finally lazmi chly ga agr hum as ko likhy ga.. chy error ay ya na ay.
	- **Create our own custom Exaptation** 

---
# Day 12 - Sunday - 12 : October : 2025
---
# Day 13 - Monday - 13 : October : 2025
1. Class and Object
2. Constrictor in dart 
	- **Constrictor Types** 
	1. default constrictor
	2.  Named constrictor
3. inheritance
4. Polymorphism
	- Method Overriding (as ma hum parent aur child ma same name ka function bna data ha.  jasy hi hum child ka object bna kar as ovreide method ko call karta ha tu wo child wala call kar data ha parent wala nahi karta. as ka ya soluation ha ka hum ko child class ma SUPER kEYWORDS LAGANA PARA GA JO AS KA CHILD MA SAME OSI NAME KA METHTHOD HA AS KA ANDAR SUPER.METHODNAME likhn para ga) same as it variable ka zariya bi kar sakty ha parent aur child ma same name ka varble bna kar un ko accecc kar ksakta ha.
	- Method Overloading
5. Abstract (Data Hide Karta Ha)
	- abstract classes ka hum object nahi bna sakty
	- abstract class ma parent jo hota ha as ma hum method ko declare karta ha, phir as ko child ma ovride karna bi zarir hota ha
	- aur jo method simipe hota ha wo bi bna sakty ha
6. Interface (Rule set karta ha)
	- dart ma interface name ka keywords nahi hota
	- agr hum na kisi class ko interface ma convert karna ha tu as ko inharintace ki tarh parent child ka concept use ho gaa.. 
	- bass difrence itna sa ha ka hum inheritance ma **extend** keyword use karta ha liykn jo interface ha as ma hum na **implements**  ka keywords use karna ota ha.
	- jasy hi hum **implements**  ka keywords lagy ga jo parent ha wo interface ki trah act kara ga. aur cild class ma 1 error ay ga ka jitny bi parent class ma method ha wo sa overide hony chy child class ma.
	- interface ka jo parent ka method ha in ko child ma overide karwsakty ha liykn print nahi karta ya parnt ka method ma jo code huu. sirf child ma jo overide ho ga wo hi print kara hga.
	- Dart me **`interface` keyword nahi hota**.
    - Jab aap `implements` use karte ho, tab class ko **interface ki tarah treat** kiya jata hai.
    - Child class ko **har method implement karna zaroori hota hai**.
    - Interface me **implementation nahi hoti**, sirf **structure (rules)** hotay hain.
7. Static Variable And Static Method
	- agr hum static variable aur funcrtion bna da as ko hum object ka zariya call nahi kar sakty.
	- agr access karna ha simple class ka name likh kar dot laga ka access kar sakty ha.
	- as ka maqsad ya fada ya hota ha ka as ko 1 bar memeory allcate hoti ha, jitni bar marzi call kari ja. memary bchat ha. static method aur function
	- stic method ka andar hum dosra simple method call nahi kar sakty
	- liykn simple method ka andar hu static call kar sakty ha.
	- JAB class ko extends kar la tu jo parent ma static variable aur function hoty ha wo extends nahi hoty but access kar sakty ha class ka name use kar ka.
	- Static Method aur Variables ko Overide aur ovelod nahi kar sakty.
8. Lambda Function Or Anonymous Function ya Name ka bagr wala function, ya without name faction
9. Higher Order Function
	- Higher Order Function ya hota ha ka koe function ha wo function hi ruuren kar ray ha
	- ya koe function ha wo as a parameter bi function la ray
10. Collection
	- List
	- Set (as ma duplication nahi ho skti, aur as ma indexing nahi hoti. agr as ko acces karna ha tu loop ka use kar ka karna parta ha)
	- Map (as ko hum Hash ya dictionary bi kahty ha).
11. Mixin
	- dart ma multi inharintace allow nahi ha
	- Mixin as ki help sa hum multi inheritance kar saktyt ha
	- multi inhertance ka matlb 1 sath 2 class ko extends karan **Examele**: class A extends classB, classD (dart as trah comma laga kar 2 classs ko inhertance nahi karna data as ko karna ka liy hum mixin ka use karta ha)
	- class keywords ki jaga mixin ka use karna ha.  aur jab as ko extends karna ha tab as coma ki jaga **with** keyword laga dana ha.
# Day 14 - Tuesday - 14 : October : 2025
1. Provider
	- Single Provider Setup 
	- Multi Provider Setup
2. **ChangeNotifier** – State manage karne wali base class.
3. **ChangeNotifierProvider** – ChangeNotifier ko UI se connect karta hai.
4. **Consumer** – Widget jo provider ka data sunti (listen) aur rebuild hoti hai.
5. **notifyListeners()** 
6. **MultiProvider**
7. **Provider State Management Project**
	- Create Counter Application
	- Create a Application Increase and Decrease the Color Opacity using Slider
	- Add Favourite Items 
# Day 15 - Wednesday - 15 : October : 2025
1. Provider Project
	- Theme Changer 
	- Calculator Design (Change Dark and Light Theme, and Perform Calculation, use custom widgets like Button, use third part Library).
# Day 16 - Thursday - 16 : October : 2025
1. Provider Project
	- Mini Game Number Compression
	- Pervious work complete (Calculator) 
# Day 17 - Friday - 17 : October : 2025
1. Provider Project
	- CRUD Operation using Provider State Management
# Day 18 - Saturday - 18 : October : 2025
1. Off
# Day 19 - Sunday - 19 : October : 2025
1. Off
# Day 20 - Monday - 20 : October : 2025
1. Dart Concept Revised
# Day 21 - Tuesday - 21 : October : 2025
1. OOP Concept Revised
2. CRUD || Using Provider State Management (Read and Insert Operation) **chatgpt ki help ka bagr**
# Day 22 - Wednesday - 22 : October : 2025
1. CRUD || Using Provider State Management (Read and Insert Operation) **chatgpt ki help ka bagr**
2. dart programming problem solving (save code and question on notes)
# Day 23 - Thursday - 23 : October : 2025
1. dart programming problem solving (save code and question on notes)
# Day 24 - Friday - 24 : October : 2025
1. dart programming problem solving (save code and question on notes)
# Day 25 - Friday - 25 : October : 2025
1. dart programming problem solving (save code and question on notes)
# Day 26 - Friday - 26 : October : 2025
1. dart programming problem solving (save code and question on notes)