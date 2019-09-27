# is-A-has-A-Relation-Ship
<h1>Is-A has-A relation explained using Dog and House Example, Good Programming approach</h1>

Here, the programmer failed to understand the difference between IS-A and HAS-A relationships. 

<b>Let's take an example</b>
<b>Project Requirements:</b> Set up a system in the house to scare away a thief if they try to sneak in. The programmer browses through the existing code base and finds this class

Suppose there is class,

class House
{
}
class Dog
{
  void BarkAndScareAway();
}

<b>All good until now. But the inexperienced programmer then decides to do something like this.</b>

class House inherits Dog
{
}

It works. The house object now has a feature to bark at the thief and scare them away. But, at the same time it inherited other features of Dog, like wagging its tail, pee on 3 legs, sniffing, etc.

Here, the programmer failed to understand the difference between IS-A and HAS-A relationships. When House inherits a Dog, it’s an IS-A relationship. Or in other words, House IS A Dog. That doesn’t make any sense, does it? How can a house become a dog? How can a house wag its tail or sniff?

The correct relationship between them should be HAS-A. The house HAS A dog makes much more sense.

class House
{
    Dog guardDog;
}
Now, the house doesn’t behave like a dog. But it has a dog that the House can rely on to perform Dog functions. So, always ask this question in English to yourself before you inherit - Is <derived class> a <base class>? If that sounds insane like “Is house a dog”, then you are not supposed to inherit.
  
  
code is given in complete project.

<b>@Credits : Subith Premdas</b>
#for learning purpose
