# Design and Implementation

## Frontend

We are using Room, Mockito and the relevant Spotify, Firebase and Google Maps libraries and APIs. The app is mainly coded for Android in Kotlin using Jetpack Compose, with a little bit of code for the backendFfirebase functions in JavaScript. 

The main components are the 3 main screens : 

- The map screen displaying the beacons
- The track lists screen displaying the user's playlists
- The profile screen displaying the user profile.

There are some subscreens : 

- The login screen
- The beacon screen to show the content of a beacons
- The edit profile screen
- The loading screen

## Backend

The backend is composed of 2 big blocks :

#### Spotify

The Spotify API is mainly used to retrieve songs and create playlists from the app.

Here are the informations we need : 

- Tracks, authors, albums and user playlists informations
- On device player status (playing, skiping ...)
- Authentication with spotify

#### Firebase

There are three types of documents stored on firebase :

- Beacons 
- Profiles
- Tracks

Profiles and beacons contain tracks and need to be linked to them with firebase references. Users need to be linked to profiles to count the number of likes.

## Data Model

We collect data locally, with the different tracks player, we manage it ourselves. We are using the spotify API and firebase to store the dataobject automatically. They are stored exactly as they are stored locally, with backend and frontend variables corresponding to each other.

The different dataclasses represent objects in the application like beacons or profiles.
They each contain sub dataclasses items, like for example playlists, or for beacons track and profiles assotiations representing the liked songs by a certain profile.

Some data is stored locally, by caching the songs that were played recently using a room database.
The sharing of the actual app data is all done via firebase, the caching as well. We also have some data sent to spotify as playlists.

## Security Considerations
We will need to protect user's location, as data collected from their interactions with beacons could be used to reconstruct their path.

## Infrastructure and Deployment

The application is developed using github CI/CD tools. The CI is setup using an emulator directly on github servers. As we intend to upload the app to the Google Playstore, the CD is largely the same as other Android apps using the same schema.

## Test Plan

We have extensive end-to-end tests. And as we rely a lot on the APIs and the backend, we implemented extensive mocking of the different intefaces to enable thorough testing of the whole app.
