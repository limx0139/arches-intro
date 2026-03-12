---
title: "Database Modification"
teaching: 10 # teaching time in minutes
exercises: 5 # exercise time in minutes
---

:::::::::::::::::::::::::::::::::::::: questions 

- How to add, modify and maintain Resources in the Arches database?

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: objectives

- Add and modify resources to the database through workflows and direct interaction with models.

::::::::::::::::::::::::::::::::::::::::::::::::

# Introduction

So far, we have covered how you would go about searching for information in Arches, but a database is only as good as its ability to keep itself up to date. In this lesson, we will learn to modify data on the Arches database.

Arches provides 2 ways to modify information in the database, through modifying the resource model tree directly or through workflows.

https://arches.readthedocs.io/en/latest/developing/extending/extensions/workflows/

Workflows are a streamlined way to modify the database designed to abstract away from working with Arches Resource Models themselves, which can end up being quite unwieldy. 

However, workflows may not be implemented for every necessary operation on the database so interacting with resource model trees is still necessary.

Here, we will use the Arches for Science Demo, which is a Arches instance designed to manage heritage science data: https://afsdemo.archesproject.org 

This Demo contains information about research done on heritage ceramic artefacts using the Arches for Science Resource Package.

To note, modifications to Arches Demos are local to each session, so while we can edit the database to have a feel for the software, no one else can see our changes and they will be reset when we leave the webpage. On an actual Arches installation,  changes made to the database will be persistent.

## Using Workflow

Lets record a scientific project onto the database. First, we navigate to find the list of Projects in the database.

![](images/04-01-Projects.png)

We find that projects have a name, a description, a list of physical objects involved, a start date, and a team.

We are tasked with recording a new project onto the database: 

- This project investigates the material composition of ceramics around different areas of the world to establish possible connections between pottery making methods across different communities. 
- The project is kindly funded by the International Foundation for Pottery Heritage.
- The name of the project is : Necessary Rudiments for Robust Ceramic Making Methods
- Earliest Start Date is 11 March 2026.
- Individuals involved are Wendy Rigter, Peter Grave and Ben Marsh.
- The Pottery objects that are studied:

| List.         | Object        |   Location  |
| ------------- |:-------------:|   -----:    |
| 1             | Sherd 782     | Kinet Höyük |
| 2             | centered      |         $12 |
| 3             | are neat      |          $1 |

## Modifying Entries Manually