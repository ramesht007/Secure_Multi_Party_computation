## What is? Secure Multi_party_computation

### Let's Consider 

- A set of parties with private inputs.
- Parties wish to jointly compute a function of their inputs sa that certain security properties are preserved.
- Properties must be ensured even if some of the parties maliciously attack the protocol
- Can model any cryptographic task

For Example: Companies that donot want to share their data to their potential compatitors or security agencies that work on
  the idea of sharing as much less data as possible.
  
## Application
- Election
- Auction
- Private database search
- Privacy-preserving data mining
- Secure set intersection (Tool and Application both)
- Much much more

## Security Requirements
### -- Consider a secure auction (with secret bids):
 - An adversary may wich to learn the bids of all parties
 - To prevent this, we require **PRIVACY**.
 
 - An adversary may wish to win with a lower bid than the highest
 - To prevent this, we require **CORRECTNESS**.
 
 - But, the adversary may also wish to ensure that it always gives the highest bid
 - To prevent this, we require **INDEPENDENCE OF INPUTS**.

 - An adversary may try to abort the execution if its bid is not the highest
 - We require **FAIRNESS**.

## General Security Propeties

Form the above discussion we get the following security properties
- **Pirvacy**: only the output is revealed
- **Correctness**: the function is computed correctly
- **Independence of inputs**: parties cannot choose inputs based on other's input
- **Fairness**: if one party recevies output, all receive output
- **Guranteed output delivery**

## Defining Security
### Option_1: Analyse security concerns for each sepcific problem
- Auctions: as in previous heading
- Elections: privacy, correctness and fairness only (?)
#### Problems:
- How do we know that all concerns are covered?
- Definitions are application dependent and need to be redefined from scratch
  for each task. 
### Option_2: General definition that capture all (most) secure computation tasks
**- Properties of any such definition**
- Well-defined adversary model
- Well-defined execution setting
- Security gurantees are clear and simple to understand
