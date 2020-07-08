# Modeling Adversaries

## Adversarial behavior

**Semi-honest:** Follows the protocol specification
- Tries to learn more than allowed by inspecting transcript

**Malicious:**  Follows any arbitrary strategy.

**Covert:** Follows any arbitrary strategy, but is averse to being caught...... 

### For Example:
- Two Hospitals want to carry out secure computation over the unoin of their databases but they donot trust each other as the hospitals 
might not want to have a sneak peak over the data and they might not even try. But we cannot say the same for the IT depratment they might 
try to get hands on some of the data form the other hospital. One does not want their's hospitals data to lie around in someone else server.
This type is called **semi-honest** Adversaries.

- Their is a group of companies that is trying to carry out computations over their combined data and there is a rule if one of the company cheats it will be kicked out of the colaboration. So the company may be restrcits itself from attacking or may weight its profits over loss from cheating. This type of adversary comes under **Covert** adversary. 

## Adversial power
- **Polynomial-time:** computational security
- **Computationally unbounded:** Information-theoretic security

## Corruption strategy
- **Static:** The set of corrupted parties is fixed before the execution begins.
####### For Example:
Here the adversary can choose who to corrupt. This can be termed as modern hacking attack, where the attacker can break into a machine which suits it's needs. Supose, there is a portocol where we choose 100 parties and out of them we choose 5 parties for main
computation, so the attacker may attack these 5 parties to get probable chance of successful attack.

- **Adaptive:** The adversary can corrupt parties during the execution, based on what has happened.(Quit harder comapred to static)
- Models modern "hacking"
- cannot use strategies that choose a small set of representatives to compute for all
- In general, **much harder!**
