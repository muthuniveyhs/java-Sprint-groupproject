<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>Task Manager</title>

  <!-- Bootstrap CSS -->
  <link
    href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css"
    rel="stylesheet"
  />
</head>
<body class="bg-light">

<div class="container mt-5">
  <h2 class="mb-4">Task Form</h2>

  <!-- Task Form -->
  <form id="taskForm" class="card p-4 mb-4">
    <div class="mb-3">
      <label class="form-label">Task Name</label>
      <input type="text" id="name" class="form-control" />
      <small class="text-danger" id="nameError"></small>
    </div>

    <div class="mb-3">
      <label class="form-label">Description</label>
      <textarea id="description" class="form-control"></textarea>
      <small class="text-danger" id="descriptionError"></small>
    </div>

    <div class="mb-3">
      <label class="form-label">Assigned To</label>
      <input type="text" id="assignedTo" class="form-control" />
      <small class="text-danger" id="assignedToError"></small>
    </div>

    <div class="mb-3">
      <label class="form-label">Due Date</label>
      <input type="date" id="dueDate" class="form-control" />
      <small class="text-danger" id="dueDateError"></small>
    </div>

    <div class="mb-3">
      <label class="form-label">Status</label>
      <select id="status" class="form-select">
        <option value="">Select status</option>
        <option>TODO</option>
        <option>IN PROGRESS</option>
        <option>REVIEW</option>
        <option>DONE</option>
      </select>
      <small class="text-danger" id="statusError"></small>
    </div>

    <button type="submit" class="btn btn-primary">Add Task</button>
  </form>

  <!-- Task List -->
  <h3 class="mb-3">Task List</h3>
  <div class="list-group" id="taskList">
    <!-- Sample Cards (minimum 5) -->
    <div class="list-group-item card mb-2">
      <div class="card-body">
        <h5 class="card-title">Sample Task 1</h5>
        <p class="card-text">Description example</p>
        <p>Assigned To: John</p>
        <p>Due Date: 2026-02-10</p>
        <span class="badge bg-secondary">TODO</span>
      </div>
    </div>

    <div class="list-group-item card mb-2">
      <div class="card-body">
        <h5 class="card-title">Sample Task 2</h5>
        <p class="card-text">UI Design</p>
        <p>Assigned To: Alex</p>
        <p>Due Date: 2026-02-12</p>
        <span class="badge bg-warning">IN PROGRESS</span>
      </div>
    </div>

    <div class="list-group-item card mb-2">
      <div class="card-body">
        <h5 class="card-title">Sample Task 3</h5>
        <p class="card-text">API Integration</p>
        <p>Assigned To: Sam</p>
        <p>Due Date: 2026-02-15</p>
        <span class="badge bg-info">REVIEW</span>
      </div>
    </div>

    <div class="list-group-item card mb-2">
      <div class="card-body">
        <h5 class="card-title">Sample Task 4</h5>
        <p class="card-text">Testing</p>
        <p>Assigned To: Nina</p>
        <p>Due Date: 2026-02-18</p>
        <span class="badge bg-success">DONE</span>
      </div>
    </div>

    <div class="list-group-item card mb-2">
      <div class="card-body">
        <h5 class="card-title">Sample Task 5</h5>
        <p class="card-text">Deployment</p>
        <p>Assigned To: Leo</p>
        <p>Due Date: 2026-02-20</p>
        <span class="badge bg-secondary">TODO</span>
      </div>
    </div>
  </div>
</div>

<!-- JavaScript file -->
<script src="script.js"></script>
</body>
</html>
