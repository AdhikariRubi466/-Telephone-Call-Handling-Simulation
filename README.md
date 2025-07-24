#  Telephone System Simulation (Lost & Delay Call Handling)

A Java-based **Discrete Event Simulation (DES)** system that simulates the working of a telephone network. It helps analyze how incoming calls are handled under two models: **Lost Call System** and **Delay Call System**

### Key Performance Metrics

|  Metric              |  Description                                                                 |
|------------------------|--------------------------------------------------------------------------------|
| Total Processed Calls  | Total number of attempted calls (valid or invalid)                            |
| Completed Calls        | Number of successfully connected and completed calls                          |
| Blocked Calls          | Calls rejected instantly due to unavailable links                             |
| Busy Calls             | Calls rejected due to all destination lines being busy                        |
| Delayed Calls          | Calls queued because lines or links were unavailable                          |
| Lost Calls             | Calls dropped from queue due to timeout or overflow                           |
| Avg. Waiting Time      | Time spent in queue before call gets connected                                |

### Project Structure

```bash
SimulationOfTelephoneSystem/
├── SimulationOfTelephoneSystem.java  # Main entry point
├── Home.java                         # Main menu navigation
├── LostCall.java                     # Immediate rejection if no link or busy line
└── DelayCall.java                    # Queuing model for delayed calls
