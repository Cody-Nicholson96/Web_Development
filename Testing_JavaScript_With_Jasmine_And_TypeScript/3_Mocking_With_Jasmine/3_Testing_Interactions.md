# Testing Interactions

In the _Virtual_Dog project, there are three throw event interactions: the static DogController receives configurations from two configuration files passed into the constructor (one-way read only), the DogController has a private method called fetch that is a listener for the master thrower event - the fetch method receives the event as a parameter when the event is triggered, the DogObject gets passed as a parameter to the DogController when an event triggers when the fetch method receives the dog object and then calls its chewOn() method which is the method we will spy on.