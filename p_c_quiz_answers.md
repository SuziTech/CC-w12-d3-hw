# Polymorphism & Composition Homework - Quiz

# Polymorphism

1. What does the ___word___ 'polymorphism' mean?

Answer: The word means 'many forms'.

2. What does it mean when we apply polymorphism to OO design? Give a simple Java example.

Answer: In OO design polymorphism means to allow different implementations of methods with the same signature.

Example:

class Animal {
  public void animalMakesASound() {
    System.out.println("Most animals make some kind of sound.");
  }
}

class Cat extends Animal {
  public void animalMakesASound() {
    System.out.println("The Cat makes: meow.");
  }
}

class Hamster extends Animal {
  public void animalMakesASound() {
    System.out.println("Hamsters rarely make a sound.");
  }
}

3. What can we use to implement polymorphism in Java?

Answer: Method overriding and method overloading can be used in Java to implement polymorphism.

4. How many 'forms' can an object take when using polymorphism?

Answer: An individual object can only take one form. Objects are not polymophic.

5. Give an example of when you could use polymorphism.

Answer: See the example in Question 2.

# Composition

6. What do we mean by 'composition' in reference to object-oriented programming?

Answer: Composition allows you to model a 'has-a' relationship between objects. It describes a class that references objects of other classes by instance variables.

7. When would you use composition? Provide a simple example in Java.

Answer: When you are modelling such relationships from the 'real' world. For example, a guitar has strings.

8. What is/are the advantage(s) of using composition?

Answer: The main advantages of using composition are code reuse, stronger encapsulation and easier maintenance.

9. When an object is destroyed, what happens to all the objects it is composed of?

Answer: the objects it is composed of can be destroyed as well. However, this needs careful consideration, as some objects in the composition may have a life after a composing object is destroyed so should not be destroyed. Not sure how language/oop model specific this behaviour is?
