# Design and Implementation

## Frontend

*List the key libraries, languages, components used by the MVP.*

*If applicable, describe essential screens.*

## Backend

The backend is composed of 2 big blocks :

#### Spotify

The spotify API is mainly used to retreive songs, we have to capacity to create playlists from the app as well.

Here are the informations we need : 
- Tracks, authors, albums and user playlists informations
- On device player status (playing, skiping ...)
- Authentication with spotify

#### Firebase

3 types of things stored on firebase :
- Beacons 
- Profiles
- Tracks

Profiles and beacons contain tracks and need to be linked to them with firebase references. Users need to be linked to profiles to count the number of likes.

## Data Model

*What data are you collecting / managing?*
We collect data locally, with the different tracks player, we manage it ourselves. We are using the spotify API and firebase to store the dataobject automatically. They are stored exactly as they are stored locally, with backend and frontend variables corresponding to each other.

*How is it organised?*
The different dataclasses represent objects in the application like beacons or profiles.
They each contain sub dataclasses items, like for example playlists, or for beacons track and profiles assotiations representing the liked songs by a certain profile.

*Where is it stored?*
Some data is stored locally, by caching the songs that were played recently using a room database.
The sharing of the actual app data is all done via firebase, the caching as well. We also have some data sent to spotify as playlists.

## Security Considerations
Because we use the location, people will be concerned by this.
We don't store the location online but we store who share which songs on which beacon, which has a location.
This means that the profiles that are not public shouldn't be shown

## Infrastructure and Deployment

The application is developed using github CI/CD tools. The CI is setup using an emulator directly on github servers. As we have to send the app to the google store the CD is largely the same as other android app using the same schema.

## Test Plan

We have extensive end-to-end tests. And as we use a lot the APIs and the back end, we have extensive mocking of the different intefaces to have thourough testing of everything on the app. 
The UI is using the maps API so we have to also testing as much as possible.

