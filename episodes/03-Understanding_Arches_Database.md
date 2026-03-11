title: "Using Markdown"
teaching: 20 # teaching time in minutes
exercises: 10 # exercise time in minutes
---
:::::::::::::::::::::::::::::::::::::: questions 

- How does the Arches Database work?

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: objectives

- Learn the structure of the Arches Database.
- Understand how its customisability allows for flexible data storage in just about any format.

::::::::::::::::::::::::::::::::::::::::::::::::

# The Arches Database.

A database is simply a way to store persistent information on a server, information that is shared and can be modified between users and periods of time. Databases are used all over web development, even on Arches itself, several discrete databases are used. For instance, to store login credentials and most importantly for heritage data storage. 

While it is not strictly necessary to have a complete understanding of the database as an end-user of Arches, some understanding of it is beneficial to understand its flexibility in design for heritage storage solutions.

The Arches database uses a graphical method of storing data that is proprietary to Arches and designed specifically for the use on heritage data in mind.

![](images/03-01-Arches_Structure_v1.png)

The above diagram shows a hierarchical structure of the Arches database. 

The Resource Package is the database structure itself, tailored for each use case. A Resource Model is the structure of a type of entry in the database, for instance, a person or an organisation or a artefact. Resource Models are designed to fit the data available in the raw data used, if we have information on when an organisation was formed and when it is disbanded, the Resource Model for an organisation may include fields to reflect that. A Resource is an instance of an object adhering to a particular Resource Model. Jon Doe being an instance of a Person Resource Model for instance. An Arches installation has 1 Resource Package containing multiple Resource Models, each of which will contain multiple Resources.

For instance, suppose we were to define a database to store the list of passengers and crew abroad the Titanic. We might want to add Resource Models to fit the people abroad the ship, along with information about their names, places of origin, whether they survived the sinking, etc. We may also include information about the different lodgings abroad the ship, as well as the different types of passangers as well as recovered artefacts from that time period. A rudimentary design for this may look like this.

![](images/03-02-Titanic_Example.png)

This Resource Package has 3 different Resource Models, for People, the Lodgings available as well as the Groups involved on the ship. Of which, instances of the lodging may include First, Second and Third Class rooms, and the Groups include Passengers and Crew. These are Instances of Resource Models. We also illustrate the structure of the Resource Model for People to contain their names, lodgings, group and fate. 

Under this structure, an instance of a Person recorded in the database may include their name, the type of room they were staying in, whether they were passenger or crew and whether they survive the tragedy.

# Exercise: Intuition for Resource Models.

In this section, we shall provide a description of an item and as an exercise, we ask how might a Resource Model of this item would look like. 

![](images/Pokemon/Pikachu.png)

(Pen and Paper)
A card collector is interested in keeping track of his collection of Pokemon cards digitally. According to the image of the Pokemon Card above, how might the Resource Model for a Pokemon Card look like?

Answer:


# Conclusion

As has been demonstrated, the Arches database is flexible and malleble to varied needs, even outside of heritage preservation and research. While as end-users, we do not directly interact with database structure, it is useful to know how it works and why it is designed in this way. 