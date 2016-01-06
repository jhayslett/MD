#Reactive Programming#
#####By: Jacob Hayslett#####

Think of the experience of purchasing a vehicle brand new. The vehicle has never been turned on, it has only been rolled off a trailer in that spot you get to turn it on for the first time. You excitedly jump inside the vehicle and go to start the engine up. As you turn the key you see the dashboard light up and all the gauges turn on. The speedometer is stuck at the “0”, the tachometer pops up to the “1", the fuel gauge rolls all the way up above the “F” symbol and finally you notice the temperature gauge move up slightly to the low section. But then all of a sudden you are devastated as you notice the gauges are stuck. You just bought a brand new vehicle and there is already something defective. You get out of the vehicle and walk back into the dealership quickly and find the guy who sold you the vehicle and ask, “Why are my gauges not working?” and he quickly responds dramatically by saying, “Because the gauges use Functional Programming!”.

This is obviously not what the salesmen would say to you but this is a great form of describing the opposite of Functional Programming, **Reactive Programming**.

Reactive Programming is a concept of programming that reacts instantaneously by altering data.

Lets compare and apply Reactive Programming to driving a vehicle. When you want to formulate how fast you are going, you would have to calculate your rate of speed, otherwise known as miles per hour(_mph_), using distance and time.

> r = d/t.

So if I am wanting to figure out my mph I would have to calculate my distance divided by my time. Lets say if I was going:

![Distance Traveled](http://hayslett.xyz/md/distanceTraveled.jpg)

**r = d/t**  
Time(_t_) = .5, for half an hour, since our measurement of rate is miles per hour.  
Example 1: Distance(_d_) = **10** miles so 10/.5 = **20mph**  
Example 2: Distance(_d_) = **20** miles so 20/.5 = **30mph**  
Example 3: Distance(_d_) = **30** miles so 30/.5 = **60mph**

Inside most vehicles there is something that uses the concept of Reactive Programming. It calculates the distance your tires are traveling along with the time to calculate your mph. This is obviously the speedometer.

Usually in your vehicle there are multiple sets of Reactive Programming such as the:

**speedometer** - speed of your vehicle  
**tachometer** - RPM or revolutions per minute  
**fuel** - percentage of fuel in tank  
**temperature** - temperature of engine coolant  

![Instrument Panel](http://hayslett.xyz/md/instrumentPanel.jpg)

The instrument panel on your dashboard can be considered the type of programming language that is selected to formulate Reactive Programming as a concept. Each gauge is using a different formula compared to example earlier of the equation to calculate miles per hour. r = d/t.

Reactive Programming is allowing the gauges in your vehicle to constantly keep you updated as a driver or passenger on all different types of information to keep you safe on the road. Without this information constantly being updated it could put you in some less than ideal situations. Without your speedometer you would have no clue how fast your are going, so you might start getting speeding tickets more frequently. Without your tachometer you wouldn’t know how hard you are pushing your engine, so you could wear parts and fluids quicker by running at higher RPMs. Let’s just say you'd be calling AAA more frequently by running out of fuel or burning up your engine.

This is just one example of the benefit to the concept of Reactive Programming.
