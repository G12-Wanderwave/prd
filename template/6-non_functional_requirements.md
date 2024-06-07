# Non-Functional Requirements

## Security, privacy, and data retention policies

Before releasing the app, we will need to make sure that it complies with many different legal frameworks, such as LPD[^1], GDPR[^2] or CCPA[^3] to only name a few.

In our app we allow user to choose whether or not they are visible by others, with what we called "private mode". This still allows music-sharing, but anonymously. Currently all user data is stored in their profile, which means that deleting it is sufficient to completely erase a user's data.

On the client-side, we require access to the user's location and notifications. Whilst we don't store any location data directly (all computations happen on the client), using data from the beacons (such as songs dropped and retreived) could theoretically allow to reconstruct a user's path. Therefore it will be very important to secure that information as well.

[^1]:https://fedlex.data.admin.ch/eli/cc/2022/491
[^2]:https://gdpr-info.eu/
[^3]:https://oag.ca.gov/privacy/ccpa


## Adoptions, Scalability and Availability

Most of the usage will likely be during peak commuting hours and increase linearly with population density. We also expect higher usage in summer due to the fact that people tend to go out and travel more during that time.
With this in mind, we will need to ensure that our backend can handle wide traffic pattern variations, both at a daily and yearly scale.