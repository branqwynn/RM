-- Radar Map Application

Design Document

Brandon Nguyen

** Introduction
Searching for the best place to play? Radar Map can help you:
- Find parks and attractions and record them in your search
- Find the restrictions zones
- Monitor the weather at your current position

Use your to search any parks and attractions near your position. For example, Summit Park is one of the best places to play with them because of its massive open area. Receive warnings on being under a restriction zone and show the its level. Noftify you when rain, ice/snow, or high winds are moving to your current position.
** Storyboard

** Function Requirements
**** Scenario
As a user, I want to search any parks and attractions that are the best places to launch without any difficulties.

**** Dependencies
Parks and Attractions search data are available and accessible.

The device has GPS capabilities and the user has granted location access.

All restriction areas and levels are present on the map.
**** Assumptions
The terrain on the map is flat.

Security sensitive locations are highlighted in different colors to show their restriction levels.

The weather is clear in the user's location.

**** Examples
1.1

**** Given GPS details and weather patterns are available 
****When I search "Addison Park"
**** Then I should receive

Name: Addison Park

Category: Park

Current Weather: Rain
-----------------------------------------------------

** Class Diagram
 ![UML](https://user-images.githubusercontent.com/55035232/106397933-f8525680-63dd-11eb-88f1-f94e0094307a.png)
 (desc)
- MainActivity: A map with the weather radar to show the current positions of rain, ice/snow, or winds depending on the setting
- MainViewModel: A screen that shows the main overview of the map
- MapView: A screen that shows the overview of the map
- Park: Noun class that represents a park
- SpecificPark: Noun class that represents a specific park
- OutsideWeatherFeed: Output database of the weather that is outputted
- ParkDatabase: Database of the different parks


** Scrum Roles
- DevOps/Product Owner/Scrum Master: Brandon Nguyen
- Frontend Developer: N/A
- Integration: N/A

Meeting times
- Myself
