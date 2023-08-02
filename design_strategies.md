<h1> Design strategies </h1>

<ol><li>What do we mean by coupling and cohesion when discussing structured design?</li>
<p>Coupling - Looks at and measures dependency <strong>between</strong> modules. The more modules are dependent on each other, the harder it becomes to implement and maintain the code, as this would suggest that we must know about module y in order to understand module x , this would be high coupling. So looks for independency between modules, so when a change in a module occurs it has little to no impact on another module, achieving low coupling.
<p>Cohesion - Looks at and shows the relationship <strong>within</strong> modules and represents the functional strength of modules. Have an aim for togetherness in a module, hoping for the module to focus on a single function, in other words high cohesion. 
<p>For structured design high cohesion, low coupling is optimal as the design aims for reduced complexity.

<li>What is the difference between top-down and bottom-up design? Which best describes a function oriented design?</li>
<p> Top-down: This approach starts at the highest level module with an overview of the system being the initial thought. The problem is then broken down into parts, and then further broken down into parts/fragments, with new broken down parts becoming less complex at each stage of refinement. This 'breaking down' occurs until the parts can no longer be fragmented, where the lowest level of modules is reached.
<p> Bottom-up: This approach, as suggested, starts from the bottom. It initially designs and solves the most fundamental parts of the problem, these parts are then combined, by grouping parts to form the next higher level modules and so on in order for the parts integrate, completing the solution ending up at the highest level. 
<p> Function oriented esign uses top-down approach.

<li>In which design methodology would a class diagram be most useful?</li>
<p> A class diagram would be most useful in object oriented programming. As it is a great tool to display the links and relationships between classes as well as detailing their properties and methods.

<li>What are the four pillars of object oriented programming? </li>
<p>Abstraction- Used when you don't have to understand exactly what the program is directly doing, so can hide away the logic of the program, instead of forcing the user to understand it.
<p>Encapsulation- removing access to parts of the code, this can be restricting properties (private) so they can only be accessed through methods within that same class, this prevents properties being overwritten for example.
<p>Inheritance- This allows for an object to acquire the properties and methods of another object, being named respectively as a parent <em>(superclass)</em> and a child <em>(subclass)</em>. Where, in order to justify inheritance, a parent class may require to have most of the functionality of the child class.
<p>Polymorphism- It uses methods that have been inherited (via inheritance) to perform different tasks, so can have a single action that can perform in different ways.

<li>What is the strategy pattern? How would its implementation differ between a functional and object oriented system?</li>
<p> Strategy- Allows for us to change the behaviours of an algorithm at runtime, meaning algorithms can be interchangeable at run time. In object oriented design you may use an interface to allow for implementing of each possible algorithm / scenario, this will enable selection of algorithms at runtime. For OOP to implement a strategy pattern, new classes and interfaces will need to be created. For a function oriented system, you can implement different versions of an algorithm inside a function which may point to functions in the selected scenario. This may be accomplished by using a function with a switch, where in each of the cases <em>(A single case repesents a scenario)</em> it will call the appropriate functions.

<li>Imagine your is creating a new online payment system. In order to gain maximum market share it can't be tied to a particular sector - it needs to work just as well when ordering a takeaway as when buying a new coat. Which design methodology would you suggest following?</li>
<p>For this scenario I think adopting an object oriented design would be best, although functional design would also work well. Modularity in the program would be important in allowing for the program to have different uses across the different sectors, as you can reuse objects that are relevant in each scenario, which can be implemented through use of an interface <em>(could use a strategy pattern)</em>. The four pillars of OOP would help enable the system to work in different sectors, for example polymorphism can be used so that an action can be performed in different ways <em>(eg like an output that is relevant to want is being brought)</em>. 