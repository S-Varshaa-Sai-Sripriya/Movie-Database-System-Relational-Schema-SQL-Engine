# MovieVerse: Movie Database System Relational Schema & SQL Engine

A fully normalized SQL-based movie database system built from scratch. Designed to simulate real-world entertainment data operations — including movies, genres, user reviews, roles, cast/crew, and award metadata — using advanced relational modeling, constraints, and procedural logic.

![Gemini_Generated_Image_biitu6biitu6biit](https://github.com/user-attachments/assets/3daabac2-6c4b-434c-9299-2104ab359333)

> 🎓 Final Project: Database Management | Stony Brook University

---

## 🧱 Schema Overview

This database supports the core structure of a real-world movie review platform. It includes entity-relationship modeling converted to SQL, with strong emphasis on:

- ✅ Relational normalization (3NF+)
- ✅ Primary and foreign key integrity
- ✅ Many-to-many mapping with junction tables
- ✅ Procedural logic with triggers & stored procedures

---

## 📁 Schema Components

| Entity           | Description |
|------------------|-------------|
| Movie          | Stores metadata for each film |
| Genre        | Genre classification linked to each movie |
| Person        | Contains actor, director, and writer identities |
| Role           | Maps people to movie roles (actor, director, etc.) |
| Review         | Stores ratings and comments by users |
| Award          | National & international awards associated with movies |
| User_Account   | Basic user management & reviewers |
| Movie_Genre    | Many-to-many between Movie and Genre |
| Movie_Award    | Many-to-many between Movie and Award |

---

## ⚙️ Key Features

- 🔐 **Triggers**: Prevent illegal review ratings or insertion of invalid dates
- 📜 **Stored Procedures**:  
  - InsertMovie — modular movie + genre + role setup  
  - InsertReview — review system with business logic  
  - GetRecommendedMovies — simple user-specific suggestion engine
- 🧹 **Validation**: Genre/award duplication, date constraints, null-safe checks
- 🧪 **Sample Data Insertion Scripts** provided

---

## 🧪 SQL Techniques Demonstrated

- Declarative schema creation (`CREATE TABLE`, `ALTER`)
- Transaction-safe stored procedures and conditional logic
- `BEFORE INSERT`, `BEFORE UPDATE` Triggers for field-level validation
- Indexing, constraints, `IF EXISTS`, `SIGNAL SQLSTATE` error throws
- Modular SQL design for reusability

---

> Also developed a basic web interface to showcase the graphical outputs.
