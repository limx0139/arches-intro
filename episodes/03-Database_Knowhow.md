---
title: "Database Basics"
teaching: 15 # teaching time in minutes
exercises: 5 # exercise time in minutes
---
:::::::::::::::::::::::::::::::::::::: questions 

- How does the Arches Database work?

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: objectives

- Learn the structure of the Arches Database.
- Understand how its customisability allows for flexible data storage in just about any format.

::::::::::::::::::::::::::::::::::::::::::::::::

## Database Basics.

A database is simply a way to store persistent information on a server, information that is shared and can be modified between users and periods of time. Databases are used all over web development, even on Arches itself, several discrete databases are used. For instance, to store login credentials and most importantly for heritage data storage. 

A good database structure is good because it is well planned out enough and does not have to be changed. As such, an end-point user will likely not have to work with the Arches database structure all that much. Regardless, understanding of it is beneficial to understand its flexibility in design for heritage storage solutions as well as understand what the database can and cannot do. This is also important for Harry to design his rare coin database!

![Harry thinking about his database](fig/Misc/Thinking_thought_bubble.png)

Given the fact that designing the database involves deciding how data is stored, you can imagine that it would not exactly be ideal to redesign the database while there is data in it, as it would involve changing the structure of all resources currently stored in it. 

## Arches Database.

The Arches database uses a graphical method of storing data that is proprietary to Arches and designed specifically for the use on heritage data in mind.

![Arches Structure](fig/03-01-Arches_Structure_v1.png)

The above diagram shows a hierarchical structure of the Arches database. 

The Resource Package is the database structure itself, tailored for each use case. A Resource Model is the structure of a type of entry in the database, for instance, a person or an organisation or a artefact. Resource Models are designed to fit the data available in the raw data used, if we have information on when an organisation was formed and when it is disbanded, the Resource Model for an organisation may include fields to reflect that. A Resource is an instance of an object adhering to a particular Resource Model. Jon Doe being an instance of a Person Resource Model for instance. An Arches installation has 1 Resource Package containing multiple Resource Models, each of which will contain multiple Resources.

For instance, suppose we were to define a database to store the list of passengers and crew abroad the Titanic. We might want to add Resource Models to fit the people abroad the ship, along with information about their names, places of origin, whether they survived the sinking, etc. We may also include information about the different lodgings abroad the ship, as well as the different types of passangers as well as recovered artefacts from that time period. A rudimentary design for this may look like this.

![Example: The Titanic](fig/03-02-Titanic_Example.png)

This Resource Package has 3 different Resource Models, for People, the Lodgings available as well as the Groups involved on the ship. Of which, instances of the lodging may include First, Second and Third Class rooms, and the Groups include Passengers and Crew. These are Instances of Resource Models. We also illustrate the structure of the Resource Model for People to contain their names, lodgings, group and fate. 

Under this structure, an instance of a Person recorded in the database may include their name, the type of room they were staying in, whether they were passenger or crew and whether they survive the tragedy.

Naturally, this is not exhaustive. Other relevant categories such as nationality or gender and familiar relations can be added. We can also include workers of Harland and Wolff, the company responsible for the construction of the ship, as well as artefacts associated with and retrieved from the ship.

So, a relationship graph for a person resource in this database may look like this:

![Jon Doe's Relations](fig/03-03-Person.png)

This describes a John Doe who is male, Irish, boarded the ship as a member of the crew, stayed in third-class lodging, who died in the sinking of the ship.

## Exercise: Intuition for Resource Models.

In this section, we will help Harry design his database. He wants to put in as much information about the coins as possible. For inspiration he pulls out a coin from his wallet:

<!-- ![Pokemon Card: Pikachu](fig/Pokemon/Pikachu.png) -->
![Harry's Coin](fig/Misc/Back_of_Bulgarian_1_euro_coin.png)

It is a Bulgarian 1 Euro coin, minted in 2026 in Bulgaria, featuring Saint Ivan of Rila the patron saint of Bulgaria and founder of the Rila Monastery. This is  designed by Petar Stoikov, who has designed several other Bulgarian coins. Naturally, the coin is minted in Bulgaria, minted from copper and nicket. As it is minted recently and as it is minted for currency, the mintage is in the millions. Given that the coin is not rare, its value is the same as its face value, 1 Euro.



# Conclusion

As has been demonstrated, the Arches database designed is flexible to varied needs, even outside of heritage preservation and research. While as end-users, we do not directly interact with database structure, it is useful to know how it works and why it is designed in this way. 