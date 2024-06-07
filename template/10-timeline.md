# Timeline/resource planning

## Execution Roadmap

The development of the MVP is scheduled to span a duration of 14 weeks. This timeline encompasses the initial setup, the development phase, testing, deployment, and the iterative process of refining features to achieve a product-market fit. We anticipate several key milestones along the way to evaluate our progress. The team, composed of 4 members, includes a part-time frontend developer, a backend developer, a part-time UI/UX designer, and a software tester who also handles DevOps.

#### Milestone 1

Design Completion and Backend setup

- Documentation of Spotify's APIs
- Documentation of Google maps APIs
- Basic UI elements are working : 
  - The google maps API is used to show a basic map
  - Basic UI elements like songs displays and lists
- Figma mockups and user flow documents
- Tests to populate the UI with songs
- Tests to check the APIs status

| **Sprint/Week Number** | **Objective** | **Outcomes** |
| --- | --- | --- |
| Week 1 | Kickoff and Documentation | API Investigation, Documentation and Scraping prototype scripts; set up project framework |
| Week 2 | Design and Technical Setup | Initial wireframes, and user flows created, started UI mockups with UI elements for plugins. Configure google maps and firebase |
| Week 3 | Design Finalization & Application Skeleton | Finalized UI/UX designs, set up development environments, and backend APIs to populate simple UI elements. |

#### Milestone 2

Beacon Development

- Start with developing the beacons frontend and backend.
- Start basic refinement of the UI for beacons and related screens
- Firebase is implemented and used

| **Sprint/Week Number** | **Objective** | **Outcomes** |
| --- | --- | --- |
| Week 4 | Beacons on a map | The beacons can now be shown on the map and can contain basic data like songs and likes. The beacons have correct location |
| Week 5 | Beacons are integrated with spotify | Songs are show on the beacon screen and can be played when clicking on them, the backend of spotify is connected |
| Week 6 | Firebase, songs UI and player | Beacons now can play songs. The player is shown when a song is played. Firebase is containing the beacons, the songs are stored on firebase and linked to the beacons |
| Week 7 | Unit and Integration Testing | Write all remaining unit tests, check frontend-backend integration with Integration tests. |

#### Milestone 3

Internal Testing and Pre-Launch Preparation


- Run end-to-end tests for several devices, fine tuning the UI
- Set up simple error handling for App and backend
- Set up Google Analytics to track user events, setup analytics dashboard, and ensure correct tracking behavior.

| **Sprint/Week Number** | **Objective** | **Outcomes** |
| --- | --- | --- |
| Week 8 | Internal Testing & Analytics/Monitoring pipelines | Thorough internal testing, Ui and APIs testing |
| Week 9 | Pre-Launch Preparations | Final bug fixes and optimizations, prepared app store and launch materials. |

#### Milestone 4

Initial Rollout and Feature Iterations for PMF

- Rollout app to alpha testers
- Marketing the app to spotify

| **Sprint/Week Number** | **Objective** | **Outcomes** |
| --- | --- | --- |
| Weeks 10-11 | Initial Rollout / Alpha Testing | Deployed app to production, monitored app performance, and gathered user analytics/insights and feedback. Start contacting spotify to show early product. |
| Week 12 | Feature Iteration 1 | Identifying drop-off points, optimizing user experience, rollout updates, improving UI, possibly |
| Week 13 | Beta Testing | Initiate marketing, getting users on the app, promptly addressing feedback to gain trust |
| Week 14 | Full Rollout | Press marketing pedals, offering incentives to join the app - free meals to lucky winners, |

## Development Resources

The primary cost of development of the product comes from developer cost. We estimate the need to secure 4 months of cash for a 4-person team to meet planned and unplanned scenarios. Because this project is backend oriented, where we need to deal with multiple APIs, we would need two full-time developers (one on backend, one on software tester+devops), along with two part time contractors for UI design and Frontend. We expect the contractors to contribute a total of 2 person-months each, over the 4-month development + GTM timeframe.
 We overprovision cash for a total of 4 person-months to meet unexpected deviations from our envisioned roadmap, those hours should be reserved by preference to front end as the schedule seems tight for 3 person-month. 

| **Function** | **Required person-months** |
| --- | --- |
| Frontend Android Developer | 3 |
| Backend Developer | 4 |
| UI/UX Designer | 2 |
| Software Tester | 4 |
| Surplus Cash Reserves | 3 |

## Deployment Resources

We will need upfront capital for the purchase of 2 MacMini so that one can serve as a redundant replica in case of hardware failures. We will need the different APIs plans, depending on the userbase we will probably need to have the plan upgraded to paid plans, the app can support a few hundred users before being paid. After which we will need to go to paid plans 

| **Item** | **Cost / unit** | **Units** | **Totals** |
| --- | --- | --- | --- |
| MacMini | 500 CHF | 2 | 1000 CHF |
| Firebase | Blaze plan | 1 | 0 CHF |
| Google maps | Free Tier | - | 0 CHF |
| Spotify | Free Tier | 1 | 0 CHF |
| TOTAL | 1000 CHF |

## Maintenance and Upkeep

As we are using mainstream APIs, the downtime should be extremely minimal. The schematics of the app are entirely decided by us and should be modified only when we decide it.
The goal is to sell the app to spotify in 4 months. Assuming we manage it, we should only have to pay the developers without too much maintenance.

