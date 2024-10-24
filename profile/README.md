# Space Finder

> "Where Learning Finds Its Place"

Space finder is classroom allocation made simple. It allows teachers to book their class locations easier and allows the locations to be displayed on the school screens.

## Context
Our school is broken up into 8 different commons (houses), and each class is fixed inside a common (except for special cases such as music which is in the music room). In each common, there are around 6 spaces where a class can take place. Every day, each class takes place in their fixed common, however the space is not fixed and needs to be booked ahead of time. The old method of how our school managed this was through a google sheet. Basically each teacher would go through and book where their class was for each period around a week before the class. This is only half the system however, the other half is letting other teachers, and the students where their classes will be. This is done through whiteboards in every common.

This system has several problems. The first being that there is no validation or checking done on the google sheets. A teacher can forget to book a class, or book the same place as another teacher and nothing would be done. Furthermore, there is nothing in place if a teacher forgets to book. The other side of the problem is displaying these classes. Teachers need to write every day on the whiteboards where each class is, for each period. Often teachers only write the data for their own class leaving students confused to where to go. This problem is made worse due to the whiteboards being very small and also hard to read at times.

This is where my project - SpaceFinder comes in. My project allows teachers to book their classes on a web interface with very minimal effort required. It also has many features to adapt to the school. It also has validation and handles issues like conflicts or cases when a teacher wants to request a space that another teacher has already booked. My project also solves the issue of whiteboards but instead automatically showing the relevant classroom allocations on the digi screens. The digi screens are screens installed in every common in our school that show events and information. My project automatically updated these screens when a new period begins to show the locations for each class.

## Features
SpaceFinder has a custom made authentication system to ensure that users data is stored securely and that no outside people can mess with the system. It uses a role based system where higher roles can perform more operations.

Spacefinder has a page to display all the teachers classes and timetables, if a user is admin they can view other teachers classes and book on their behalf.

Spacefinder uses an admin panel to allow the admins to configure details such as term dates, add or remove teachers or leaders and other details about the system. They also have granular control of the timetable structure as they are able to remove or add periods, classes and also provide different timetable structures for different weeks. For example, they can provide an empty timetable on half days and holidays. They could also set the year 12s and 13s to study leave while keeping the year 11 timetable normal etc.

Spacefinder has a page to book classes. Teachers can pick their class and make their bookings for the week. If theres a spot they want thats taken, they can request for it from the other teacher. The system handles or validation and ensures no errors or conflicts.
At the very start of the next week Monday 12 am, the system runs a check to see all periods not yet booked, and assigns them each a space based on factors such as class size and availability. This results in there never being any unbooked periods.

Spacefinder also links with the screens to display the period about 5 min before each class.

## Plan

![](https://raw.githubusercontent.com/Space-Finder/.github/main/profile/assets/Architecture.png)