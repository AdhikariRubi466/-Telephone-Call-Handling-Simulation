# Telephone-Call-Handling-Simulation
# Project Structure

### 1. Welcome.java — Main Entry Point  
**Purpose:** Launch screen with a telephone-themed interface.

**Features:**  
- Two navigation buttons:  
  ➤ LostCallSystem  
  ➤ DelayCallSystem  
  
### 2. LostCallSystem.java — Lost Call Simulation  
**Objective:** Models scenarios where calls may be dropped due to system limitations.

**Components:**  
- **Call Queue Table:** Displays call info (From, To, Duration, Arrival Time)  
- **Line Status Table:** Indicates the state of 8 telephone lines (Busy / Free)  
- **Active Calls Table:** Shows up to 3 ongoing calls  
- **Call Counters:** Tracks Processed, Completed, Blocked, Busy calls  
- **Link Utilization Panel:** Max Links vs Used Links  
- **System Clock:** Real-time ticking clock  

### 3. DelayCallSystem.java — Delayed Call Simulation  
**Objective:** Simulates delayed call handling with enhanced queue management.

**Additional Features:**  
- Same tables and indicators as in LostCallSystem  
- Extra support for delayed call queuing  
- Implements custom call processing algorithms  

##  Shared Functionalities  

###  Menu Bar (Available in All Windows)  
- **About Us:** HTML-formatted version info + developer credits  
- **Help:** User guide with instructions and troubleshooting  

##  Simulation Mechanics  

###  Call Generation  
- Randomly generated calls with varying lengths and arrival times  
- Queue auto-refill system for continuous simulation  
- Arrival patterns managed with a time-based scheduler  

###  UI Feedback  
- Color-coded Tables: For call and line status  
- Real-Time Clock: Continuously updated simulation time  
- Auto Refresh: Tables and indicators update dynamically  

##  Technical Details  

###  Core Technologies  
- **Java Swing:**  
  - JFrame — Main windows  
  - JTable — Data displays  
  - JMenuBar — Menus  
  - JOptionPane — Dialog messages  

- **Simulation Engine:**  
  - Timer-based call events  
  - Priority queues for efficient call management  
  - Stateful tracking of line and call usage  

###  Window & Lifecycle Management  
- Uses `DISPOSE_ON_CLOSE` to close child windows without terminating the main app  
- Maintains parent-child relationships between Welcome screen and simulations  

##  How to Run the Project  
1. Launch the simulation by executing `Welcome.java`.  
2. Choose your mode: Lost Call or Delay Call.  
3. Observe real-time call handling simulation.  
4. Use menu options for help and contact info.  

##  Learning Highlights  
This project demonstrates:  
- Real-world simulation principles  
- Event-driven programming  
- State management  
- GUI design using Java Swing 
