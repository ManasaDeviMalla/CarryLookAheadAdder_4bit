What is a Carry Look-ahead Adder?

A digital computer must contain circuits which can perform arithmetic operations such as addition, subtraction, multiplication, and division. Among these, addition and subtraction are the basic operations whereas multiplication and division are the repeated addition and subtraction respectively.To perform these operations ‘Adder circuits’ are implemented using basic logic gates. 

Adder circuits are evolved as Half-adder, Full-adder, Ripple-carry Adder, and Carry Look-ahead Adder.

Among these Carry Look-ahead Adder is the faster adder circuit. It reduces the propagation delay, which occurs during addition, by using more complex hardware circuitry. It is designed by transforming the ripple-carry Adder circuit such that the carry logic of the adder is changed into two-level logic.

In this adder, the carry input at any stage of the adder is independent of the carry bits generated at the independent stages. Here the output of any stage is dependent only on the bits which are added in the previous stages and the carry input provided at the beginning stage. Hence, the circuit at any stage does not have to wait for the generation of carry-bit from the previous stage and carry bit can be evaluated at any instant of time.

In  Carry Look-ahead Adder two new terms are introduced 

– Carry generate and carry propagate. 

Carry generate Gi =1 whenever there is a carry Ci+1 generated. It depends on Ai and Bi inputs. 
Gi is 1 when both Ai and Bi are 1. 

Hence, Gi is calculated as Gi = Ai. Bi.

Carry propagated Pi is associated with the propagation of carry from Ci to Ci+1. It is calculated as Pi = Ai ⊕ Bi. 

Using the Gi and Pi terms the Sum Si and Carry Ci+1 are given as below –

Si = Pi ⊕ Gi.

Ci+1 = Ci.Pi +Gi.

Therefore, the carry bits C1, C2, C3, and C4 can be calculated as

C1 = C0.P0+G0

C2 = C1.P1+G1 = ( C0.P0+G0).P1+G1

C3 = C2.P2+G2 = (C1.P1+G1).P2+G2

C4 = C3.P3+G3 = C0.P0.P1.P2.P3 + P3.P2.P1.G0 + P3.P2.G1 + G2.P3 + G3

It can be observed from the equations that carry Ci+1 only depends on the carry C0, not on the intermediate carry bits.


Advantages of Carry Look-ahead Adder:

In this adder, the propagation delay is reduced. The carry output at any stage is dependent only on the initial carry bit of the beginning stage. Using this adder it is possible to calculate the intermediate results. This adder is the fastest adder used for computation.
