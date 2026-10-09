# CSC 2560 Agent Lab Part 2
## Design Notes

### 1. What problem are we solving?
Students sometimes have trouble finding information about different services on campus. The goal of this project is to create an AI assistant that helps students find locations, hours, and contact information for places like the library, tutoring center, academic advising, and financial aid office.

### 2. Why can't Gemini answer campus questions by itself?
Gemini can answer general questions, but it might not have accurate or updated information about my college. By connecting it to a JSON file with campus information, the assistant can give answers based on information we provide instead of guessing.

### 3. Why use JSON instead of putting everything in Python?
First, JSON keeps the campus information separate from the Python code. Second, it makes information easier to update without changing how the agent works. Third, it keeps the information organized so we can add more campus resources later.

### 4. Three limitations and possible improvements
One limitation is that campus information can change. In the future, the information could be updated automatically from the college website.

Another limitation is that the assistant only knows about resources included in the JSON file. We could improve this by adding more verified campus resources.

A third limitation is that the assistant currently uses a basic testing interface. In a future lab, we could build a website that makes it easier for students to use.

### 5. What happens if the JSON information is wrong?
If the information is incorrect, students could go to the wrong location, call the wrong number, or show up when an office is closed. Whoever maintains the campus resource information is responsible for checking it against official college sources and keeping it updated.

### Campus Resource Research

| Resource | Location | Hours | Phone | Email | Website | Verified By | Date Verified |
|---|---|---|---|---|---|---|---|
| Library | Hultquist Library, Jamestown Campus | Check official website | 716.338.1008 | Not listed | https://www.sunyjcc.edu/support/learning-commons/library/ask | JCC website | 2026-10-09 |
| Tutoring Center | HULT Floor 1, Learning Commons | Appointments through Starfish | 716.338.1008 | Not listed | https://www.sunyjcc.edu/support/learning-commons/learning-center/tutoring | JCC website | 2026-10-09 |
| Academic Advising | Success Center, COCE Floor 1 | Contact office | 716.338.1065 | successcenter@mail.sunyjcc.edu | https://www.sunyjcc.edu/support/success-center/advising | JCC website | 2026-10-09 |
| Financial Aid Office | COCE Floor 1 | Contact office | 716.338.1009 | FinancialAid@sunyjcc.edu | https://www.sunyjcc.edu/support/financial-aid-billing | JCC website | 2026-10-09 |