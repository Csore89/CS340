# CS340

CS-340: Client/Server Development Portfolio

1. Writing Maintainable, Readable, and Adaptable Programs

To write programs that are maintainable, readable, and adaptable, I rely heavily on the Separation of Concerns and Object-Oriented Programming (OOP).

During this course, I developed a CRUD (Create, Read, Update, Delete) Python module in Project One, which acted as a standalone Data Access Layer for a MongoDB database. In Project Two, I imported this module into a Dash web application.

Advantages: The primary advantage of this architecture is that the dashboard's user interface (the front-end) does not need to know the complex details of how MongoDB works. It simply calls the read() method from my module. This makes the dashboard code much shorter, cleaner, and easier to read.

Adaptability & Future Use: Because the CRUD module is completely independent of the dashboard, it is highly adaptable. In the future, I could reuse this exact same Python module to connect the Austin Animal Center database to a mobile application, a REST API, or a completely different web framework (like Django or Flask) without changing a single line of the database logic.

2. Approaching Problems as a Computer Scientist

As a computer scientist, I approach problems using Decomposition—breaking a massive, overwhelming project into small, manageable layers. For the Grazioso Salvare project, I separated the client's request into three distinct pieces:

The Data (Model): Storing and querying the shelter data efficiently using MongoDB.

The Logic (Controller): Writing Python callbacks to filter the data based on rescue types (Water, Mountain, Disaster).

The Interface (View): Designing a user-friendly layout with Dash, Plotly, and Leaflet maps.

How this differed from previous assignments: Previous coursework often focused on isolated scripts running in a terminal. This project required a "Full-Stack" mindset, where I had to consider how data flows from a back-end database, through a Python server, and into a front-end web browser dynamically.
Future Strategies: In the future, when designing databases for clients, I will start by analyzing the specific questions the client wants answered (e.g., "Which breeds are best for water rescue?"). I will use those requirements to dictate my database schema and indexing strategies, ensuring the database is optimized for the exact queries the application will run.

3. The Role of Computer Scientists and the Value of this Project

Computer scientists do much more than write code; they build systems that translate massive amounts of raw, chaotic data into actionable human insights. Our job is to automate tedious processes so that users can make faster, more accurate decisions.

For a company like Grazioso Salvare, this work is transformative. Before this dashboard, identifying potential search-and-rescue dogs would require manually sorting through thousands of CSV rows, looking for specific breeds, ages, and genders a slow process prone to human error.

By delivering an interactive, click-driven dashboard, the Grazioso Salvare staff can now instantly filter the database and physically locate candidate dogs on a geographic map. This efficiency saves the organization countless hours of administrative work, allowing them to focus their resources on what truly matters: rescuing animals, training them, and deploying them to save human lives.
