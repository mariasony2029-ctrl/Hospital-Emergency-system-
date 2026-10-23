# Smart Hospital Emergency Resource Management System (ERMS)

## Project Overview
The Smart Hospital Emergency Resource Management System is an academic demonstration project for managing emergency patient queues and tracking selected hospital resources.

It demonstrates:
- **Priority-based patient queue:** Patients are listed by severity: Critical, Urgent, then Stable. Patients with the same severity retain registration order.
- **Binary Search:** Patient records are searched by Patient ID after sorting the IDs.
- **Resource tracking:** Available ICU beds and ventilators can be viewed and updated.

> **Important:** This is a classroom demonstration only. It is not intended for real clinical use or to make medical triage decisions.

## Project Files

| File | Purpose |
|---|---|
| `index.html` | Website structure and interactive dashboard |
| `style.css` | Dashboard layout, colors, cards, tables, and responsive styling |
| `HospitalERMS.java` | Standalone Java console program demonstrating patient priority management, binary search, and resource tracking |
| `README.md` | Project overview, setup instructions, features, and limitations |

## How to Run the Website

1. Download `index.html` and `style.css`.
2. Place both files in the same folder.
3. Open `index.html` in a modern browser such as Google Chrome.
4. Register patients, search by Patient ID, remove patients, and update resource counts.

The website uses JavaScript embedded in `index.html` for browser interactions. The `style.css` file controls the appearance.

## How to Run the Java Program

Install a Java Development Kit (JDK), then:

1. Open a terminal or command prompt in the folder containing `HospitalERMS.java`.
2. Compile the program:

   ```bash
   javac HospitalERMS.java
   ```

3. Run it:

   ```bash
   java HospitalERMS
   ```

4. Select a menu option:
   - `1` — Register an emergency patient
   - `2` — Display the priority queue
   - `3` — Search for a patient by ID using Binary Search
   - `4` — Update ICU bed and ventilator availability
   - `5` — View resource availability
   - `0` — Exit

The Java program starts with three sample records: P101, P102, and P103.

## Features

- Register patients with ID, name, age, and severity.
- Display patients in priority order.
- Search for patients by ID using Binary Search.
- Remove patients from the browser dashboard.
- Track available ICU beds and ventilators.
- Use a responsive dashboard on desktop and mobile screens.

## Data-Structure Concepts

### Priority Queue
Severity levels used in this demonstration:
- `1` — Critical
- `2` — Urgent
- `3` — Stable

A lower severity number is given higher queue priority. This is a simplified academic model, not a validated clinical triage protocol.

### Binary Search
Binary Search is performed on patient records sorted by Patient ID. Sorting is required for Binary Search to work correctly.

## Limitations

- The HTML dashboard and Java console program run independently.
- Website patient data is held only in browser memory and is lost when the page is refreshed.
- The Java program does not save records to a database.
- The website is not connected to the Java program. Connecting them requires a Java backend (such as Spring Boot or Servlets) and an API.
- Resource counts are manually updated and are not connected to actual hospital systems.

## Future Enhancements

- Connect the website to a Java backend through REST APIs.
- Store patient and resource records in a database.
- Add secure login and role-based access.
- Add audit logs and stronger input validation.
- Use a clinically approved workflow before adapting the project for real healthcare use.

## Technologies Used

- HTML5
- CSS3
- JavaScript for browser-side dashboard interactions
- Java for the standalone console implementation
- Java Collections Framework (`ArrayList`, `Comparator`)

## Author Details
Before submission, add your name, team members, department, college, and academic year.
