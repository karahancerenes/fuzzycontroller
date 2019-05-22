# Fuzzy controller implementation by using skfuzzy library &amp; Python

![fuzzy_ee](https://user-images.githubusercontent.com/33702287/58201783-9d96cb00-7cde-11e9-96c3-fbb26e1b03f5.png)

![fuzzy_controller](https://user-images.githubusercontent.com/33702287/58201819-b3a48b80-7cde-11e9-9430-4bd0ce4746ba.png)

Introduction

An artificial world has been created by some villains. The shocking(!) news is that their aim is to conquer the whole galaxy via the artificial world. The artificial world is very similar to ours and in that World there live human-like biological beings called bots. They are creatures equipped with artificial intelligence without soul. Bots attack the planets in the galaxy to serve their masters. Thus, the planets including ours are in danger. However, our scientists and politicians have found a way to turn this situation into our advantage. They have analyzed that bots can get sick and dealing with sick bots becomes easier. Hence, they have developed a virus. Moreover, they have placed an undercover agent among the villains and that agent have founded a medicine company to sell the cure to the bots. Hence, the bots implicitly contribute to our economy by buying the medicines. In this way, we can make more investments for the developments which will protect our world from villains.

The point of the story is creating a plague in the artificial world and controlling it is utterly severe. In this homework, you will create a plague by spreading your virus throughout the artificial world. Your aim is to infect 60% of the bots in the world and maintain that percentage. In this way, your disease will not be considered significant enough by the authorities to develop a permanent cure for it and there will always be customers to your medicines.

You infect the bots by contaminating the environment with your virus. Assume that you have conducted the required research on the relation between the infection rate and the contamination amount by considering the birth-death rates as well. Hence, you are able control the infection rate in terms of percentage per day. In that manner, setting infection rate to some x % day means that the percentage of the infected bots will be increased by x; namely, if the current percentage were p then the percentage after a day would be p+x. On the other hand, your research has revealed that there exists a disappearance rate for your virus owing to the symptoms of your disease and natural birth-death rates. The disappearance rate is proportional to the percentage of the infected bots. The more bots get infected, the more rapidly vanished your disease will be. You can also measure that rate in terms of percentage per day. Therefore, there is an effective infection rate which is the difference between the infected rate controlled by you and the disappearance rate. Your task is to provide proper control for the infection rate so that the percentage of the infected bots is to come to the equilibrium at 60% as quickly as possible. You will perform this task via Fuzzy Control! You see that coming...


Input Variables and Control Variable

The input variables are the two measurements which are the current percentage of the infected bots,

π∈[0,1] 

and the current effective infection rate,

(π ) ̇∈[-1,1]

The control variable,

δ ∈[-0.15,0.15]

is the infection rate to be added to the current infection rate. Note that the control variable allows to increase or decrease the infection rate and its maximum magnitude is limited to 0.15.

Task: Implementing a fuzzy controller which takes two input measurements and provides one output control to quickly infect 60 % of the bots and maintain that percentage.

Fuzzy Partitioning

![infection](https://user-images.githubusercontent.com/33702287/58202500-6a553b80-7ce0-11e9-808c-a8b5362564d3.png)

![control_variable](https://user-images.githubusercontent.com/33702287/58202528-7e993880-7ce0-11e9-9fad-cb506e49f649.png)

Results

![plague](https://user-images.githubusercontent.com/33702287/58202548-8658dd00-7ce0-11e9-9973-3df9644bcd92.png)
