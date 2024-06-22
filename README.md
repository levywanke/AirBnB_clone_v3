
### Project Outline and Steps

#### 1. Fork and Set Up Repository
- Fork the existing AirBnB clone repository to your GitHub account.
- Rename the repository to `AirBnB_clone_v3`.
- Update the README.md:
  - Add yourself (Levy Wanyonyi, Alvin Muhindi) as authors.
  - Describe your contributions and improvements to the project.

#### 2. Improve Storage (Task 2)
- Update `DBStorage` and `FileStorage` classes with new methods (`get` and `count`) in the `storage_get_count` branch.
- Implement these methods to retrieve objects and count objects in storage.
- Write unit tests for these methods in `tests/test_models/test_engine/test_db_storage.py` and `tests/test_models/test_engine/test_file_storage.py`.

#### 3. Set Up API (Tasks 3, 4, 5)
- Create an API structure using Flask:
  - Create folders and files:
    - `api/__init__.py`
    - `api/v1/__init__.py`
    - `api/v1/app.py`
    - `api/v1/views/__init__.py`
    - `api/v1/views/index.py` (for status endpoint)
    - `api/v1/views/states.py` (for states endpoint)
    - `api/v1/views/cities.py` (for cities endpoint)
- Define endpoints:
  - `/api/v1/status` for API status (`index.py`)
  - `/api/v1/stats` for statistics (`index.py`)
  - Error handling for `404 Not found` (`app.py`)
  - CRUD operations for States (`states.py`) and Cities (`cities.py`) using RESTful principles.

#### 4. Documentation and Testing
- Ensure PEP 8 style compliance.
- Document all modules, classes, and functions.
- Write extensive unit tests using `unittest` module.
- Organize tests in the `tests` folder as per the project structure.
- Ensure all tests pass using `python3 -m unittest discover tests`.

#### 5. Deployment and Submission
- Test your API endpoints using `curl` commands or a tool like Postman.
- Deploy your application locally or to a cloud server for testing.
- Create a pull request on GitHub and request a review from your peer (Levy or Alvin).
- Verify that all project requirements and tasks are completed before submission.

### Example Repository Structure

```
AirBnB_clone_v3/
│
├── api/
│   ├── __init__.py
│   └── v1/
│       ├── __init__.py
│       ├── app.py
│       ├── views/
│       │   ├── __init__.py
│       │   ├── index.py
│       │   ├── states.py
│       │   └── cities.py
│
├── models/
│   ├── engine/
│   │   ├── __init__.py
│   │   ├── db_storage.py
│   │   └── file_storage.py
│   └── __init__.py
│
├── tests/
│   ├── test_models/
│   │   ├── test_engine/
│   │   │   ├── test_db_storage.py
│   │   │   └── test_file_storage.py
│   └── test_api/
│       ├── test_v1/
│       │   ├── test_index.py
│       │   ├── test_states.py
│       │   └── test_cities.py
│
├── README.md
└── requirements.txt
```

### Next Steps
- Start by setting up your project structure and files as outlined.
- Implement each endpoint and functionality incrementally.
- Test thoroughly and ensure documentation and PEP 8 compliance.
- Collaborate closely with your teammate (Levy or Alvin) to review each other's code and merge pull requests.
