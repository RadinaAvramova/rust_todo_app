# Rust Todo App
Welcome to the Rust Todo App! This project is a simple todo list application built with Rust, allowing users to create, read, update, and delete tasks. With the Rust Todo App, users can efficiently manage their tasks and stay organized.

## Features
1. **Task Management:** Allows users to perform CRUD operations (Create, Read, Update, Delete) on tasks, including adding new tasks, viewing existing tasks, updating task details, and deleting tasks.

2. **Task Prioritization:** Supports prioritization of tasks by assigning them different priority levels such as high, medium, or low, helping users focus on important tasks and manage their workload effectively.

3. **Task Status:** Tracks the status of tasks (e.g., pending, in progress, completed) to provide users with visibility into the progress of their tasks and help them stay on top of their commitments.

4. **Task Categories:** Enables users to categorize tasks into different categories or tags (e.g., work, personal, shopping) to organize tasks by context or purpose and facilitate easier navigation and filtering.

5. **Task Due Dates:** Allows users to set due dates and deadlines for tasks, helping them prioritize tasks and manage their time efficiently by focusing on urgent or time-sensitive tasks.

### Running it

Clone or download this repository.

You need to have cargo-web installed as well as a suitable target for the Rust compiler to generate web output. 
By default cargo-web uses asmjs-unknown-emscripten. 

#### Rust stable

Install cargo-web and the asmjs and wasm32 emscripten targets as follows:

```
$ cargo install cargo-web
$ rustup target add asmjs-unknown-emscripten
$ rustup target add wasm32-unknown-emscripten
```

For normal Debug build run 
```
$ cargo web start
```

To run an optimised build instead of a debug build use:

```
$ cargo web start --target-webasm-emscripten=wasm32-unknown-emscripten --release
```

#### Rust nightly
If you are using rust nightly you can use the brand new `wasm32-unknown-unknown` target

```
$ cargo install cargo-web
$ rustup target add wasm32-unknown-unknown
$ cargo web start --target-webasm=wasm32-unknown-unknown
```

## Usage
1. **Add Tasks:** Use the appropriate command or option to add new tasks to the todo list, providing task details such as title, description, priority, due date, and category.

2. **View Tasks:** View the list of tasks currently stored in the todo list, including details such as title, priority, status, due date, and category.

3. **Update Tasks:** Update existing tasks by modifying their details such as title, description, priority, due date, status, or category as needed.

4. **Delete Tasks:** Remove tasks from the todo list by deleting them individually or in bulk, allowing users to declutter their list and focus on active tasks.

5. **Filter and Sort Tasks:** Apply filters or sorting options to the task list to narrow down tasks based on criteria such as priority, due date, status, or category, enabling users to find specific tasks quickly.

## Customization
You can customize the Rust Todo App by modifying aspects such as the user interface design, task management features, data storage options, and additional functionality such as task reminders or notifications. Additionally, you can integrate with external libraries or services to enhance the application's capabilities.

