PROMPT 1:
-------------------------------------------------------------------------------------------------------------------
Build a single Volt single-file component that manages a task list, backed by a MySQL table through Eloquent.

It must:

List all tasks.
Create a task from a title input. An empty title must be rejected with a validation error and must not be saved.
Toggle a task between complete and incomplete.

[[[https://chat.deepseek.com/a/chat/s/b0533dd9-eadc-48f3-8155-32b712dc736f](https://chat.deepseek.com/share/m3j9fmnkb6w6o9esab)]()](https://chat.deepseek.com/share/m3j9fmnkb6w6o9esab)

PROMPT 2:
-------------------------------------------------------------------------------------------------------------------
A migration creates a tasks table with these columns: id, title (string), completed (boolean, default false), created_at, updated_at.

A Task Eloquent model (App\Models\Task) with title and completed mass-assignable.

A Volt component named tasks (file: resources/views/livewire/tasks.blade.php) mounted at the route /tasks, with:

a public property $title (string),
a method addTask() that validates title as required|string|max:255, creates the task, and resets $title,
a method toggle($id) that flips that task's completed value.
The provided Pest suite (tests/Feature/TaskListTest.php) checks all of the above. Do not edit the test file.

[https://chat.deepseek.com/a/chat/s/b0533dd9-eadc-48f3-8155-32b712dc736f](https://chat.deepseek.com/share/m3j9fmnkb6w6o9esab)
