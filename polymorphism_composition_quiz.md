# Polymorphism & Composition Homework - Quiz

# Polymorphism

1. What does the ___word___ 'polymorphism' mean? 
	
	Polymorphism is derived from the Greek terms poly and morph, which means many and form, respectively. So polymorphism means many forms, which is why it is applied to OOP, as some classes can be programmed to have "many forms".

2. What does it mean when we apply polymorphism to OO design? Give a simple Java example.

	A simple Java example of polymorphism would be if we had an abstract class called Vehicle, and several different classes inheriting from Vehicle, such as Car, Truck, GolfCart, and Van. The superclass Vehicle has a method called drive(), so the classes that inherit from it also have that method. But when drive() is implemented in the subclasses, it can be overriden in order to perform a different functionality than in the superclass, which leads to different behavior in one subclass from the other when the same method is called. 

3. What can we use to implement polymorphism in Java?
	
	In order to implement polymorphism in Java, we need to use utilize an abstract class, and whatever classes are to be different "forms" of that abstract class must inherit from it. Then, if desired, the methods of the abstract superclass can be overriden in one or more of the subclasses.

4. How many 'forms' can an object take when using polymorphism?

	An object can take only one form when using polymorphism. In other words, it can only inherit from one class. However, a class can extend (be inherited from) as many classes as practically. 

5. Give an example of when you could use polymorphism.

	An example of when you could use polymorphism is when you want to have a group of similar classes inherit a specific set of properties and methods from one class. This group of classes can then all have access to the properties/methods without you needing to rewrite the code. For example, the classes Student and Teacher could inherit from class Person, so they would both have a method read, but a Student might read slower than a Teacher.



# Composition

6. What do we mean by 'composition' in reference to object-oriented programming?

	Composition means that an object is composed of one or more other objects. In other words, one object has the functionality of another object.

7. When would you use composition? Provide a simple example in Java.

	In reference to the Vehicle example above, a GolfCart could inherit from the Vehicle class (so a GolfCart is a Vehicle), but it is composed of a GolfClubStorage object in the back seat (i.e. a GolfCart has a GolfClubStorage object). The GolfCart object could also have an interface called ICharger, which allows its to have access to the functionality of having its battery charged. 

8. What is/are the advantage(s) of using composition?

	One advantage of composition is that an object can only inherit from one class, but can be composed of many parts, which makes composition more flexible than inheritance.  

9. When an object is destroyed, what happens to all the objects it is composed of?

	When an object is destroyed, all of the objects that it has (i.e. is composed of) also get destroyed, since they only exist in relation to their composite object.  