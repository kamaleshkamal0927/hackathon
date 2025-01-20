<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>MindEase - Mental Wellness Companion</title>
  <link rel="stylesheet" href="styles.css">
  <script src="https://unpkg.com/lucide@latest"></script>
</head>
<body>
  <div class="app" id="app">
    <!-- Header -->
    <header>
      <div class="header-content">
        <div class="header-left">
          <i data-lucide="brain" class="logo-icon"></i>
          <h1>MindEase</h1>
          <button class="panic-button" id="panicButton">
            <i data-lucide="alert-triangle"></i>
            <span>Panic Button</span>
          </button>
        </div>
        <div class="header-right">
          <button class="theme-toggle" id="themeToggle">
            <i data-lucide="moon" class="moon-icon"></i>
            <i data-lucide="sun" class="sun-icon hidden"></i>
          </button>
          <i data-lucide="menu" class="menu-icon"></i>
        </div>
      </div>
    </header>
    <!-- Main Content -->
    <main>
      <div class="dashboard">
        <!-- Health Stats -->
        <div class="card">
          <div class="card-header">
            <h2>Health Monitor</h2>
            <i data-lucide="activity"></i>
          </div>
          <div class="health-stats">
            <div class="stat">
              <div class="stat-label">
                <i data-lucide="heart"></i>
                <span>Heart Rate</span>
              </div>
              <span class="stat-value" id="heartRate">75 BPM</span>
            </div>
            <div class="stat">
              <div class="stat-label">
                <i data-lucide="activity"></i>
                <span>Blood Pressure</span>
              </div>
              <span class="stat-value" id="bloodPressure">120/80</span>
            </div>
            <div class="stress-level">
              <div class="stress-header">
                <span>Stress Level</span>
                <span id="stressLevel">50%</span>
              </div>
              <div class="stress-bar">
                <div class="stress-fill" id="stressBar"></div>
              </div>
            </div>
          </div>
        </div>

        <!-- Breathing Exercise -->
        <div class="card">
          <div class="card-header">
            <h2>Breathing Exercise</h2>
            <i data-lucide="waves"></i>
          </div>
          <div class="breathing-exercise">
            <div class="breath-circle" id="breathCircle">
              <span id="breathCount">0</span>
            </div>
            <button class="primary-button" id="breathingButton">Start Breathing</button>
          </div>
        </div>

        <!-- Clock and Date -->
        <div class="card">
          <div class="card-header">
            <h2>Time & Date</h2>
            <i data-lucide="clock"></i>
          </div>
          <div class="clock">
            <p class="time" id="time">00:00:00</p>
            <p class="date" id="date">Monday, January 1, 2024</p>
          </div>
        </div>

        <!-- Notes -->
        <div class="card">
          <div class="card-header">
            <h2>Notes</h2>
            <i data-lucide="notebook-pen"></i>
          </div>
          <div class="notes-section">
            <div class="input-group">
              <input type="text" id="noteInput" placeholder="Add a note...">
              <button class="primary-button purple" id="addNoteButton">Add</button>
            </div>
            <div class="notes-list" id="notesList"></div>
          </div>
        </div>

        <!-- Reminders -->
        <div class="card">
          <div class="card-header">
            <h2>Reminders</h2>
            <i data-lucide="calendar"></i>
          </div>
          <div class="reminders-section">
            <div class="input-group">
              <input type="text" id="reminderInput" placeholder="Add a reminder...">
              <button class="primary-button orange" id="addReminderButton">Add</button>
            </div>
            <div class="reminders-list" id="remindersList"></div>
          </div>
        </div>

        <!-- Zen Garden -->
        <div class="card">
          <div class="card-header">
            <h2>Zen Garden</h2>
            <i data-lucide="tower-control"></i>
          </div>
          <div class="zen-garden">
            <p>Interactive Zen Garden game coming soon...</p>
          </div>
        </div>
      </div>
    </main>

    <!-- Footer -->
    <footer>
      <p>MindEase - Your Mental Wellness Companion</p>
    </footer>


  <script src="app.js"></script>
</body>
</html>
