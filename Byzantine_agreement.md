# Byzantine Generals Problem

[Link to the paper](https://people.eecs.berkeley.edu/~luca/cs174/byzantine.pdf)


Lets's say, we are in the Byzantine empire (an anicent roman empire 🏰) and it is surrounded by **n** generals. 

#### We consider:

- **n** generals, connected by **pair-wise private, authentic channel**.
- Each General has a secret plan (bit):
    - retreat (0)
    - attack (1)
- Upto **t** generals may be **traitor**.
- Goal: to come up with a **common action plan for the honest generals**.
    - Should be equal plan of the **hosnest generals** if they all had the **same individual action plan**.

#### Computer sciecne based abstraction:

- **n** mutually-distrusting parties.
- Upto to **t** corruption.
- **Goal**: to design a **distributed protocol**, allowing the **honest parties** to agree on a **common output**. 

    - (m1, m2, m3, m4, m5, ......, mn-1, mn ---> m  **[Agreement]**(all the good servers or parties at end should have a common ouput and this is agreement.)
    - (m1, m2, m3, m4, m5, ......, mn-1, mn ---> m  **[Validity]**(if all the good servers have same input.. then that should be the final output.)
    
#### Applications:
   - Secure multi-party computation (MPS) protocols.
   - State-machine replication / distributedd databases.
   
#### Some of the Widely-Studied settings:

- Level of Syncronization
- Type of faults
- Setup available
- Type of channels
