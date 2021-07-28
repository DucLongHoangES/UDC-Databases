# UDC-Databases
Boxing championship Database design. ER diagram, relational eschema and DB script


Degree in Computer Engineering
Databases – Supervised assignment: E/R
Academic year 2020/2021

This work consists of designing and implementing in Oracle a database, including the conceptual (E/R diagram), logical (relational schema), and physical (create tables) design. The steps to complete this work, and that guide the preparation of the documentation that must be submitted, are the following:

Step 1: Selection of the domain to model
Later, we present two possible topics, select one.

  Option 2 – Logistics of a boxing championship
The Galician Boxing Federation needs a database to manage clubs championships. The fights of each championship will take place over several weeks in various enclosures (sport pavilions and gyms).
1. There are a number of clubs affiliated to the Federation, which are those that can register for the championships. We want to know which boxers are part of a club at any time. We also want to know which clubs are registered in each championship, and (if you understand that by default they should not be all) which of their boxers will participate in it.
2. For each boxer, we must know her/his details such as category, weight and number of victories and defeats.
3. A championship consists of several phases, and in each phase fights are held. Each championship fight faces two boxers, and consists of a series of rounds (the number depends on the development of the fight). In the database, for each fight we want to record the location (the enclosure where it is held), the phase, the participants, the number of rounds, and who was the winner. For each round, the duration and the number of points and fouls obtained by each boxer must be recorded.
4. The fights are evaluated by judges. It is important to keep a record of the regulars and substitutes judges planned for each fight. But, it is also necessary to know who were the ones who finally participated and the scores assigned to each contestant (boxer) in each combat round.
5. We also want to use the database to plan ticket sales for the championships. Each enclosure (e.g., sport pavilions) is divided into zones, each one with a maximum number of associated locations. The price of the ticket will depend on the fight and its location within the enclosure.

Questions to answer about the domain:

a) We want to know the current composition of the federated clubs in Galicia.

b) We want to know how many victories and defeats had the boxer A along his/her career.

c) For the championship X, we want to know the clubs that participated, and their composition during the championship.

d) For the championship X, we want to know the fights that were held. For each fight, we have to obtain the participating boxers, the winner, and the venue (enclosure) where it took place.

e) For the fight C between boxers A and B, we want to know the amount of rounds, the duration of each round, the points obtained by each fighter and the fouls committed by each fighter.

f) For the fight C between boxers A and B, we want to know the judges who were planned as regulars and substitutes, and from these, we want to know who were the ones who finally covered the fight.

g) For each participating judge of the fight C between boxers A and B, we want to know how many points were given to each fighter in each round.

h) For the fight C between boxers A and B, we want to know how many tickets were available in each zone of the venue where it took place, and at what price. We also want to know how many tickets were sold in each zone.

Step 2: Conceptual design – E/R diagram
Design a conceptual model for the domain you have chosen and draw the resulting E/R diagram. You should clearly specify all types of entity (indicating whether they are strong or weak) with their attributes, as well as the types of relationship between them. Remember to include the cardinality of the relationship types, and the (total, partial) participation of the participating entity types. To do this, you must use the notation that was used in theory classes. The characteristics of entity types, relationship types, and attributes should be explained if their name is not self-descriptive.

Step 3: Logical model design – Relational schema
Transform the previous E/R diagram into the corresponding relational scheme. You should clearly specify the primary and foreign keys for each resulting relationship. The notation used in theory classes must be used.

Step 4: Oracle implementation
Create the tables specified in the relational model. You must include all relevant restrictions (primary keys, foreign keys, not null ...). Enter a small number of rows in all tables to validate that the design works properly.
You must create a script (text file) that can be executed with DBeaver (or similar) where everything is included (instructions "create table" and "insert into ... values ...").
