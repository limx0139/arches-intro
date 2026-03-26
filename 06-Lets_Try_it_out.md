---
title: "Let's Try it out"
teaching: 5 # teaching time in minutes
exercises: 15 # exercise time in minutes
---

:::::::::::::::::::::::::::::::::::::: questions 

- How would the Arches installation we will work with look like

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: objectives

- Exercise populating an Arches Database.
- Interact with and modify persistent data written by peers.

::::::::::::::::::::::::::::::::::::::::::::::::

## Local Server

For this section, we will work on a local installation of Arches, which the instructors will share a link for.

Let's get back to Harry, who after learning the Arches basics, is now ready to populate his own Arches installation. He has set up the database in episode 3 as follows:

![Coin Structure](fig/03-04-Coin_Structure.png)

Recap:
This means that there are 3 different types of resources in the database, Designers, Countries and the Coins themselves. Coins store information on its Name, Design, Mintage and Photoes of the coin as well as relations to Designers and Countries.

You will find some information on these resources in the tables below:

| Name        | Design      | Mint Date   | Mint Quantity| Face Value  | Actual Value |Designer  | Country      |
| ----------- | ----------- | ----------- | ----------- | ----------- | ----------- |----------- | ----------- |
| Belgium 2 Euros     | King Albert II and his royal monogram, the letter "A" beneath a crown       | 2004      | 10000000       | 2       | 2        | Jan Alfons Keustermans      | Belgium       |
| Croatia 50 cents      | Nikola Tesla with the Croatian checkerboard in the background.      | 2023      | 30000000       | .50       | .50 cents        |  Ivica Družak      | Croatia       |
| Croatia 1 Euro     | A marten with the Croatian checkerboard in the background.      | 2023      | 30000000       | 1       | 1        |  Stjepan Pranjković      | Croatia       |
| Croatia 5 cent      | Nikola Tesla with the Croatian checkerboard in the background.      | 2023      | 10000000       | 0.05      | 0.05        |  Maja Škripelj     | Croatia       |
| Latvia 1 Euro      | Latvian folk maide        | 2014      | 10000000       | 1      | 1       | Guntars Sietiņš       | Latvia       |
| Irish 2 Euro      | Celtic harp       | 2003      | 30000000       | 2      | 2       | Jarlath Hayes      | Ireland       |
| Irish 1 Euro      | Celtic harp       | 2003      | 30000000       | 1      | 1       | Jarlath Hayes      | Ireland       |
| Irish 50 cents      | Celtic harp       | 2003      | 10000000       | .50      | .50       | Jarlath Hayes      | Ireland       |
| Irish 5 cents      | Celtic harp       | 2003      | 5000000       | .05      | .05       | Jarlath Hayes      | Ireland       |
| Brussels Atomium Commemerative Coin      | An image of the Atomium in the center of the coin and the engraver’s initials to right with two mintmarks near the base. The outer ring of the coin features the 12 stars of the European Union, the letter ‘B’ and the year of mintage ‘2006’.       | 2006      | 20000       | 2      | 20       | Luc Luycx      | Belgium       |


<a href="fig/Coins/Coin_Photos.zip" download>Click to Download</a>


