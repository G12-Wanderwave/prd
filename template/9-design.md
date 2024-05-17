# Design and Implementation

## Frontend

*List the key libraries, languages, components used by the MVP.*

*If applicable, describe essential screens.*

## Backend

*Decompose the MVP into functional blocks.*
3 types of things stored on the back end (firebase) :
- Beacons 
- Profiles
- Tracks

## Data Model

*What data are you collecting / managing?*
We have many different dataclasses that deal with the data

*How is it organised?*
The different dataclasses represent objects in the application like beacons or profiles
They each contain sub dataclasses items

*Where is it stored?*
Everything is stored on firebase

*How is it shared/copied/cached?*
The sharing is all done via firebase, the caching as well. 

## Security Considerations
Because we use the location, people will be concerned by this.
We don't store the location online but we store who share which songs on which beacon, which has a location.
This means that the profiles that are not public shouldn't be shown

## Infrastructure and Deployment

*How is the application developed, tested and deployed?*

*Any special infrastructure requirements.*

## Test Plan

*How is the application developed, tested and deployed?*

*Any special infrastructure requirements.*

