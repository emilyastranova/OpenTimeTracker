# Contributing to OpenTimeTracker

Thank you for considering contributing to OpenTimeTracker! We appreciate your interest and welcome any contributions that help improve the project.

## Ways to Contribute

There are several ways you can contribute to OpenTimeTracker:

- Report bugs: If you encounter any issues or bugs, please [open an issue](https://github.com/tyleraharrison/OpenTimeTracker/issues) and provide detailed information about the problem.
- Suggest enhancements: Have an idea to improve OpenTimeTracker? Feel free to [open an issue](https://github.com/tyleraharrison/OpenTimeTracker/issues) and share your suggestions.
- Submit pull requests: Contributions in the form of pull requests are always welcome. If you have implemented a new feature or fixed a bug, please submit a pull request for review.

## Getting Started

To get started with contributing to OpenTimeTracker, follow these steps:

1. Fork the repository to your GitHub account.
2. Clone your forked repository to your local machine.
3. Create a new branch for your contributions.
4. Make your changes and test them thoroughly.
5. Commit your changes and push them to your forked repository.
6. Submit a pull request from your branch to the main repository's `main` branch.

## Project Structure

The following is the project structure for OpenTimeTracker:

```shell
OpenTimeTracker/
├── opentimetracker-api/
|   ├── backend/
│       ├── app.py
│       ├── api/
│       │   ├── endpoints/
│       │   │   ├── authentication.py
│       │   │   ├── time_tracking.py
│       │   │   └── ... (other API endpoints)
│       │   └── __init__.py
│       ├── models/
│       │   ├── user.py
│       │   └── ... (other data models)
│       ├── services/
│       │   ├── authentication.py
│       │   └── ... (other backend services)
│       └── utils/
│           ├── database.py
│           └── ... (other utility modules)
├── opentimetracker-web/
│   ├── public/
│   ├── src/
│   │   ├── components/
│   │   ├── routes/
│   │   ├── services/
│   │   └── main.js
│   ├── package.json
│   ├── rollup.config.js
│   └── ... (other frontend configuration files)
├── .gitignore
├── .gitmodules
├── CODE_OF_CONDUCT.md
├── CONTRIBUTING.md
├── LICENSE
├── README.md
└── requirements.txt
```

Explanation of the project structure:

- `ott_backend/`: Contains the backend code using Python FastAPI.
  - `app.py`: The entry point for the backend application.
  - `backend/`: Contains the backend source code.
    - `api/`: Contains the API endpoints.
    - `models/`: Contains the data models used in the backend.
    - `services/`: Contains the backend services that handle business logic.
    - `utils/`: Contains utility modules for the backend.
- `ott_frontend/`: Contains the frontend code using Svelte.
  - `public/`: Contains static assets and files served by the frontend.
  - `src/`: Contains the Svelte source code.
    - `components/`: Contains reusable Svelte components.
    - `routes/`: Contains the frontend routes and associated components.
    - `services/`: Contains frontend services for making API calls or handling other frontend-specific logic.
    - `main.js`: The entry point for the frontend application.
  - `package.json`, `rollup.config.js`, and other frontend configuration files.
- `.gitignore`: Specifies which files and directories should be ignored by version control.
- `CODE_OF_CONDUCT.md`: The code of conduct for the project.
- `CONTRIBUTING.md`: The contributing guidelines for the project.
- `LICENSE`: The license file for your project.
- `README.md`: The project's readme file providing an overview, instructions, and other important details.
- `requirements.txt`: Lists the Python dependencies required by the backend.

This layout separates the backend and frontend code into their respective directories, making it easier to maintain and deploy them independently. The backend focuses on the API endpoints, models, services, and utility modules, while the frontend contains components, routes, and services specific to the frontend application.

## Database Structure

The following is the database structure for OpenTimeTracker:

```shell
Table: users
+----+--------------+---------------------+
| id | name         | email               |
+----+--------------+---------------------+
| 1  | John Doe     | john@example.com    |
| 2  | Jane Smith   | jane@example.com    |
+----+--------------+---------------------+

Table: tags
+----+-------------------+
| id | name              |
+----+-------------------+
| 1  | Babysitting       |
| 2  | Freelancing       |
| 3  | Lawnmowing        |
+----+-------------------+

Table: time_entries
+----+---------+---------------+---------------------+---------------------+
| id | user_id | tag_id        | clock_in            | clock_out           |
+----+---------+---------------+---------------------+---------------------+
| 1  | 1       | 1             | 2023-05-01 08:30:00 | 2023-05-01 17:00:00 |
| 2  | 1       | 2             | 2023-05-02 09:00:00 | 2023-05-02 18:00:00 |
| 3  | 2       | 1             | 2023-05-01 09:30:00 | 2023-05-01 15:30:00 |
+----+---------+---------------+---------------------+---------------------+
```

## Code Style and Guidelines

To maintain a consistent codebase, please adhere to the following guidelines when making contributions:

- Follow the [Python PEP 8 style guide](https://www.python.org/dev/peps/pep-0008/) for code formatting.
- Write clear and concise commit messages.
- Include necessary documentation and comments for your code.

## Code of Conduct

Please note that by contributing to OpenTimeTracker, you are expected to follow the project's [Code of Conduct](CODE_OF_CONDUCT.md). We aim to create a welcoming and inclusive community for all contributors.

## License

By contributing to OpenTimeTracker, you agree that your contributions will be licensed under the project's [GNU General Public License v3.0](LICENSE).

## Contact

If you have any questions or need further assistance, feel free to reach out by [opening an issue](https://github.com/tyleraharrison/OpenTimeTracker/issues).

We appreciate your valuable contributions to OpenTimeTracker!
