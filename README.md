# WWoN_GMHelper
A GM tool for the TTRPG system, Worlds Without Number.

## Features

### World Management

The GM should be able to record and reference geographical and political data about their world. The handbook provides ample tools to assist in the creation of the data, so this app should take care of the rest. 

### NPC Management

The GM should be able to record and reference data about their NPCs.

### Adventure Management

The GM should be able to record and reference data about the adventure thus far as well as plans for the future of the adventure.

### Bestiary

The GM should be able to record and reference data about potential enemies.

## Architecture

Will be using React/Typescript.
Will abide by SOLID principles:
- **S**ingle-responsibility principle
 - There should never be more than one reason for a class to change.
- **O**pen-closed principle
 - Software entities should be open for extension but closed for modification.
- **L**iskov substitution principle
 - Functions that use pointers or references to base classes must be able to use objects of derived classes without knowing it.
- **I**nterface segregation principle
 - Clients should not be forced to depend upon interfaces that they do not use.
- **D**ependency inversion principle
 - Depend upon abstractions, not concretions.
There will be two major sections to the app: Model and View.

### Model

This section will handle data management.
Every data entity will have two classes: 
- a repository class to interact with the database
- a services class to call the repository and handle any secondary logic

### View

This section will handle the interface.
Every component will have two classes:
- a view class that defines the react component
- a controller class that handles data fetching and logic that the view class requires