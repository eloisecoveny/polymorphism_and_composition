# Polymorphism & Composition
**Quiz**

## Polymorphism

### What does the word 'polymorphism' mean?
Polymorphism is the ability for an object to take on many forms.

### What does it mean when we apply polymorphism to OO design? Give a simple Java example.
When we apply polymorphism to objects in OOP it ables us to manage and handle objects according to their abilities. For example in Java we might have several different classes that share a common behaviour. Ordinarily we would not be able to store instances of these different classes into one ArrayList, however by applying polymorphism to these objects we will be able to group them together according to their communal behaviour (this may be an Interface that each class shares).

### What can we use to implement polymorphism in Java?
Interfaces in Java can allow us to define a particular behaviour and implement this behaviour on different classes that may not share anything else in common. If several different classes implement the same Interface, we can then group instances of these different classes together, for example in ArrayLists. In this state the objects are considered objects according to their communal Interface, however they retain the data belonging to their unique class, which can be accessed by 'casting' an object instance back into an instance of its class.

### How many 'forms' can an object take when using polymorphism?
It can take on an indefinite number of forms, however an object will always be an instance of a single class.

### Give an example of when you could use polymorphism.
An example in Java might be if you had a network and a variety of different devices that can connect to that network. These devices would each belong to a different class, for example an audio output device, a printer, a mobile phone, etc. Each device however has the ability to connect, an Interface 'IConnect' could be integral to each device class. Therefore the network has the ability to detect each device as it appears in the form of an IConnect object, and it can store them within a ArrayList of IConnect objects.

## Composition

### What do we mean by 'composition' in reference to object-oriented programming?
Composition in object-oriented programming is the principle that classes can contain instances of other classes within them.

### When would you use composition? Provide a simple example in Java.
You would use composition when the integrity of contents of one class may rely on other classes of objects. For example a car could be a class, however a real-world car is comprised of many other objects, such as an engine, tyres, a gearbox, etc. An instance of a car would likely require object instances of an engine, and an instance of a gearbox, etc.

### What is/are the advantage(s) of using composition?
Advantages of using composition is it allows you to reuse code and it gives design more flexibility. It can feel more natural building classes out of various components than trying to find commonality between them and creating Interfaces. The main disadvantage with composition is that if you delete the parent class instance, the integrated class instances are also deleted.

### When an object is destroyed, what happens to all the objects it is composed of?
They are destroyed along with the parent object.

[Quiz Brief](https://gist.github.com/futuresocks/ae746a162027ab82f9a606e2c2239f27)
