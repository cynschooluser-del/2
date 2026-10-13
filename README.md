:root {
  --primary: #4f46e5;
  --primary-hover: #4338ca;
  --success: #16a34a;
  --error: #dc2626;
  --bg: #f8fafc;
  --card-bg: #ffffff;
  --text: #1e293b;
}

body {
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  background-color: var(--bg);
  color: var(--text);
  display: flex;
  justify-content: center;
  padding: 20px;
  margin: 0;
}

.quiz-container {
  width: 100%;
  max-width: 600px;
}

header {
  text-align: center;
  margin-bottom: 24px;
}

.filter-section {
  display: flex;
  align-items: center;
  justify-content: space-between;
  margin-bottom: 16px;
  background: var(--card-bg);
  padding: 12px 16px;
  border-radius: 8px;
  box-shadow: 0 1px 3px rgba(0,0,0,0.1);
}

select {
  padding: 8px 12px;
  border-radius: 6px;
  border: 1px solid #cbd5e1;
  font-size: 0.95rem;
}

.progress-bar-container {
  height: 8px;
  background: #e2e8f0;
  border-radius: 4px;
  overflow: hidden;
  margin-bottom: 20px;
}

#progress-bar {
  height: 100%;
  width: 0%;
  background: var(--primary);
  transition: width 0.3s ease;
}

.card {
  background: var(--card-bg);
  padding: 24px;
  border-radius: 12px;
  box-shadow: 0 4px 6px -1px rgba(0,0,0,0.1);
}

.card-header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 16px;
}

.badge {
  background: #e0e7ff;
  color: var(--primary);
  padding: 4px 10px;
  border-radius: 20px;
  font-size: 0.85rem;
  font-weight: 600;
}

.prompt {
  font-size: 1.25rem;
  font-weight: 500;
  margin-bottom: 20px;
  line-height: 1.5;
}

.input-group {
  display: flex;
  gap: 10px;
  margin-bottom: 16px;
}

input[type="text"] {
  flex: 1;
  padding: 12px;
  border: 2px solid #cbd5e1;
  border-radius: 8px;
  font-size: 1rem;
}

input[type="text"]:focus {
  outline: none;
  border-color: var(--primary);
}

button {
  padding: 12px 20px;
  background: var(--primary);
  color: white;
  border: none;
  border-radius: 8px;
  font-weight: 600;
  cursor: pointer;
  transition: background 0.2s;
}

button:hover { background: var(--primary-hover); }

.feedback {
  padding: 12px 16px;
  border-radius: 8px;
  margin-bottom: 16px;
  font-weight: 500;
}

.feedback.correct { background: #dcfce7; color: var(--success); }
.feedback.incorrect { background: #fee2e2; color: var(--error); }

.next-btn { width: 100%; margin-top: 10px; }
.hidden { display: none; }
