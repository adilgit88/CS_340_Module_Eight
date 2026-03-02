# CS 340 – Dashboard and Database Integration Project

## Reflection

### Writing Maintainable, Readable, and Adaptable Programs

I write maintainable and readable programs by separating responsibilities and organizing code into clear, reusable components. In this course, the CRUD Python module from Project One was a good example of that principle. Instead of embedding database logic directly inside the dashboard, I created a separate class responsible only for interacting with MongoDB. That separation made the dashboard code cleaner and easier to understand because it focused only on user interaction and visualization.

The advantage of this approach was flexibility. When I needed to query, update, or delete records, I could reuse the same CRUD methods without rewriting database logic. If database credentials or connection details change in the future, I only need to modify the CRUD module instead of editing multiple files.

This CRUD module could easily be reused in other applications. For example, it could support a web application, a REST API, or a mobile app that connects to the same database. The modular design allows it to scale beyond this one dashboard project.

---

### Approaching Problems as a Computer Scientist

I approach problems by first breaking them into smaller, manageable parts. For this project, I separated the requirements into three layers:

1. Database structure and queries
2. Data access through the CRUD module
3. Dashboard interface and filtering logic

Before building the dashboard, I tested queries directly in MongoDB to ensure they returned the correct data. Then I connected those queries through the CRUD class into Python. Finally, I integrated them into interactive dashboard components.

This approach differed from earlier programming assignments where the focus was mainly on algorithms or isolated functions. Here, I had to think about system design, data modeling, user interaction, and database performance together.

In the future, when creating databases for client requests, I would:

* Clarify requirements before designing the schema
* Normalize or structure data to support expected queries
* Test aggregation pipelines early
* Separate backend logic from frontend presentation

That structured approach helps reduce errors and improves scalability.

---

### What Computer Scientists Do and Why It Matters

Computer scientists design systems that transform raw data into useful information. In this project, the dashboard converted stored animal rescue records into searchable, filterable insights for Grazioso Salvare.

Without structured databases and efficient queries, organizations are left with static spreadsheets or disorganized records. By building a database-driven dashboard, we enable faster decision-making, improved reporting, and better operational awareness.

For a company like Grazioso Salvare, this kind of system could:

* Quickly identify animals eligible for training
* Filter by rescue type or location
* Improve response coordination
* Reduce manual data sorting

Ultimately, computer scientists build tools that increase efficiency, reduce human error, and support smarter decisions. That impact is why this work matters.

