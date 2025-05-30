# Talk to DB - Natural Language to SQL Query Converter

A Python application that allows users to query a SQLite database using natural language. The application uses Groq's language model to convert English questions into SQL queries, making database interactions more intuitive and accessible.

## Features

- Natural language to SQL query conversion
- SQLite database integration
- Streamlit web interface
- Groq AI model integration for query processing
- Student records management system

## Technology Stack

- Python 3.12+
- SQLite3
- Streamlit
- Langchain with Groq
- python-dotenv

## Project Structure

```
talk-to-db/
├── database.py      # Database setup and operations
├── main.py         # Main application logic and Streamlit interface
├── student.db      # SQLite database file
├── pyproject.toml  # Project configuration and dependencies
└── README.md      # Project documentation
```

## Database Schema

The `STUDENT` table contains the following columns:

- `NAME` (VARCHAR): Student's name
- `COURSE` (VARCHAR): Course name
- `SECTION` (VARCHAR): Section identifier
- `MARKS` (INT): Student's marks

## Setup and Installation

1. Clone the repository:

```bash
git clone <repository-url>
cd talk-to-db
```

2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Set up environment variables:
   Create a `.env` file in the root directory and add your Groq API key:

```
GROQ_API_KEY=your_api_key_here
```

4. Run the application:

```bash
streamlit run main.py
```

## Usage

1. Start the Streamlit application
2. Enter your question in natural language (e.g., "Show me all students in Data Science course")
3. The application will convert your question to SQL and display the results

## Example Queries

- "How many students are enrolled in total?"
- "Show me all students in Data Science course"
- "What is the average marks in each section?"
- "List all students with marks above 80"

## Code Formatting

This project uses Black for code formatting. To format the code:

```bash
black .
```

## TODO List for Future Improvements

1. Database Enhancements

   - [ ] Add more tables for comprehensive student management
   - [ ] Implement database migrations system
   - [ ] Add data validation and constraints
   - [ ] Create backup and restore functionality

2. Query Features

   - [ ] Add support for complex JOIN operations
   - [ ] Implement query caching for better performance
   - [ ] Add query history feature
   - [ ] Support for data visualization queries

3. User Interface

   - [ ] Add dark/light theme toggle
   - [ ] Implement user authentication
   - [ ] Create interactive query builder
   - [ ] Add export functionality for query results

4. AI Integration

   - [ ] Implement query suggestion feature
   - [ ] Add error explanation in natural language
   - [ ] Support for multiple language models
   - [ ] Add context-aware query optimization

5. Documentation and Testing

   - [ ] Add comprehensive API documentation
   - [ ] Create unit tests for database operations
   - [ ] Add integration tests
   - [ ] Create user guide with common use cases

6. Security
   - [ ] Implement SQL injection prevention
   - [ ] Add input validation
   - [ ] Create user roles and permissions
   - [ ] Add audit logging

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.
