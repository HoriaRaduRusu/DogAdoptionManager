# DogAdoptionManager
Application that manages a dog adoption centre, providing application modes for admins and users. The user can also create a list of dogs to adopt, which is stored externally.

## Used Concepts and Several Application Features
- Graphical User Interface, built using the ```QT Framework```
- Layered Architecture: ```presentation layer``` (application UI), ```business layer``` (controllers), ```persistence layer``` (repositories and model), ```database layer``` (database storing dogs)
- Usage of OOP concepts such as ```inheritance```, ```encapsulation```, ```polymorphism``` and ```inheritance```. 
- Usage of QT signals and slots
- Exceptions handling

## Design Patterns Used
- ```Model-View-Controller``` for displaying the contents of the database in the table, the photos being displayed using QT delegates
- ```Command``` design patter, used for the undo/redo functionality

## Other Application Features
- Letting the user select the application mode (```user``` or ```admin```) and, if ```user``` is chosen, what type of adoption list is wanted (```CSV``` or ```HTML```) at launch.
- Undo and Redo functionality for the features related to adding dogs to the database and adopting dogs. These also work with the usual key combinations (```CTRL - Z``` and ```CTRL - Y```).

## Admin Mode Features
- displaying a table with all the available dogs
- adding a new dog
- removing an existing dog
- updating an existing dog
- displaying statistics - a bar chart showing the quantity of dogs of each available breed

## User Mode Features
- see all of the avaiable dogs one by one. The dog's picture will be opened in the browser and their information will be shown in the application, and the user will be able to choose whether or not they want to adopt the dog before seeing the next available one. If the user reaches the last dog, the list will return to the first available one (if there still is one)
- seeing dogs filtered by breed. The above functionality works the same with the filtered list.
- see a list of the dogs they chose to adopt, along with their photos, in a table inside the application.
- see a list of the dogs they chose to adopt externally, either in a CSV or HTML file, based on the selection made at the launch of the application.
