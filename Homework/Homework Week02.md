# Homework  Week02
### Feb 21st

P2. Equation 1.1 gives a formula for the end-to-end delay of sending one packet of length L over N links of transmission rate R. Generalize this formula for sending P such packets back-to-back over the N links.  

    Solution:
    The delay of sending one packet from source to destination over a path consisting of N links each of rate R is N*L/R.
    The delay depends on how long it takes when the last packet arrives ar the destination. The last packet equivalently needs to pass (N+P-1) links to arrive. 
    So the delay is (N+P-1)*L/R.



P5. Review the car-caravan analogy in Section 1.4. Assume a propagation speed of 100 km/hour.  

a. Suppose the caravan travels 175 km, beginning in front of one tollbooth, passing through a second tollbooth, and finishing just after a third tollbooth. What is the end-to-end delay?  

b. Repeat (a), now assuming that there are eight cars in the caravan instead
of ten.

    Solution:  
    a.
    time for a car to propagate from 1st to 2nd toll both = 175km/(100km/hr) = 1.75 hr
    time to "push" entire caravan through toll booth onto highway = 12*10 = 120 sec
    end-to-end delay = (1.75 hr + 120 sec) * 2 = 214 min  
    b.
    time to "push" entire caravan through toll booth onto highway = 12*8 = 96 sec  
    end-to-end delay = (1.75 hr + 96 sec) * 2 = 213.2 min

P14. Consider the queuing delay in a router buffer. Let I denote traffic intensity; that is, I = La / R. Suppose that the queuing delay takes the form IL/R*(1 - I) for I < 1.  
a. Provide a formula for the total delay, that is, the queuing delay plus the transmission delay.  
b. Plot the total delay as a function of L / R.

    Solution:
    transmission delay = L / R
    total delay =  queuing delay + transmission delay = (1+I-I^2)*L/R = 
    L/R + a*(L/R)^2 - a^2*(L/R)^3
    It's a cubic function of (L/R).


