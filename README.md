# ShrinkLink

ShrinkLink is used for shortening long urls to share them easily on any platform.

## System Requirements

- Ruby version 3.1.1 or higher

- Rails version 7.0.4 or higher

- MySQL database

## Installation

To run the ShrinkLink on your local machine, follow these steps:

1. Clone the repository:

   ```bash
   $ git clone https://github.com/ankkyprasad/ShrinkLink.git
   ```

2. Install the necessary dependencies:

   ```bash
   $ bundle install
   ```

3. Set up the database:

   ```bash
   $ rails db:create
   $ rails db:migrate
   ```

4. Start the server:

   ```
   $ rails server
   ```

5. Open your browser and go to [Localhost](http://localhost:3000) to access the application.

<br />

## Database Schema

The ShrinkLink uses one table in the MySQL database:

### **Link Table:**

<br />

| Column name  | Data type | Constraints                 |
| ------------ | --------- | --------------------------- |
| id           | integer   | primary key, auto-increment |
| lookup_code  | string    |
| original_url | string    |
| created_at   | datetime  |
| updated_at   | datetime  |
