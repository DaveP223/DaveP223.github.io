<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>ClassWork</title>
    <style>
     /* Add your CSS styles here */
       body {
                  font-family: Arial, sans-serif;
                  text-align: center;
                  background-color: #f2f2f2; /* Light gray background color */
              }

              h1 {
                  font-size: 36px;
                  margin-top: 50px;
                  background-color: purple;
              }

              ul {
                  list-style-type: none;
                  padding: 0;
                  background-color: #ffffff; /* White background color */
                  border-radius: 10px; /* Rounded corners */
                  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1); /* Shadow effect */
                  margin: 20px auto; /* Center the list horizontally */
                  max-width: 600px; /* Limit the width of the list */
                  padding: 15px; /* Add some padding */
              }

              li {
                  font-size: 15px;
                  margin-top: 20px;
              }

              .priority-dropdown {
                  margin-left: 20px;
              }

              .completed {
                  text-decoration: line-through;
              }

              /* Add styles for celebratory animation */
              @keyframes celebration {
                  0% { transform: scale(1); }
                  50% { transform: scale(1.1); }
                  100% { transform: scale(1); }
              }
              .celebration {
                  animation: celebration 1s ease;
              }

              .priority-high {
                  color: red;
              }

              .priority-medium {
                  color: yellow;
              }

              .priority-low {
                  color: blue;
              }

              /* Style for priority dropdown */
              .priority-dropdown {
                  margin-left: 10px;
              }

              .message {
                  font-weight: bold;
                  color: green;
                  font-size: 24px; /* Adjust the font size as needed */
                  margin-top: 20px; /* Increase the margin for better separation */
                  text-align: center; /* Center-align the text */
              }

              #completedTasks {
                  margin-top: 50px;
                  background-color: 'gray'; /* White background color */
                  border-radius: 10px; /* Rounded corners */
                  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1); /* Shadow effect */
                  max-width: 600px; /* Limit the width of the list */
                  padding: 15px; /* Add some padding */
                  margin: 20px auto; /* Center the list horizontally */
              }

              .addBackButton {
                  margin-left: 10px;
                  cursor: pointer;
                  color: green;
              }

    
    </style>
</head>
<h1>To Do List</h1>
<body>
<ul>

    <li id="cardioTask">
        <details>
            <summary>Cardio: 20 Min Per Machine</summary>
            <select class="priority-dropdown" onchange="setPriorityColor(this)">
                <option value="priority-high">High</option>
                <option value="priority-medium">Medium</option>
                <option value="priority-low">Low</option>
                <option value="priority-neutral">Neutral</option>
            </select>
            <ul>
                <input type="checkbox" id="cardio1" onclick="completeAndDelete(this, 'cardioTask'); displayTaskCompleted();">
                <label for="cardio1">Treadmill</label>
            </ul>
            <ul>
                <input type="checkbox" id="cardio2" onclick="completeAndDelete(this, 'cardioTask'); displayTaskCompleted();">
                <label for="cardio2">Steps</label>
            </ul>
            <ul>
                <input type="checkbox" id="userinput1"onclick="completeAndDelete(this, 'cardioTask'); displayTaskCompleted();">
                <input type="text" name="userinput1"/>
            </ul>
        </details>

    </li>
    <li id="pushupsTask">
        <details>
            <summary>Push Ups: 50 Reps 3 Sets</summary>
            <select class="priority-dropdown" onchange="setPriorityColor(this)">
                <option value="priority-high">High</option>
                <option value="priority-medium">Medium</option>
                <option value="priority-low">Low</option>
                <option value="priority-neutral">Neutral</option>
            </select>
            <ul>

                <input type="checkbox" id="pushup1" onclick="completeAndDelete(this, 'pushupsTask'); displayTaskCompleted();">
                <label for="pushup1">Classic</label>
            </ul>
            <ul>
                <input type="checkbox" id="pushup2" onclick="completeAndDelete(this, 'pushupsTask'); displayTaskCompleted();">
                <label for="pushup2">Close Grip</label>
            </ul>
            <ul>
                <input type="checkbox" id="userinput2" onclick="completeAndDelete(this, 'pushupsTask'); displayTaskCompleted();">
                <input type="text" name="userinput2"/>
            </ul>

        </details>

    </li>
    <li id="threePtmade">
        <details>
            <summary>3pt Shots: 500 Made<input type="date"></summary>
            <select class="priority-dropdown" onchange="setPriorityColor(this)">
                <option value="priority-high">High</option>
                <option value="priority-medium">Medium</option>
                <option value="priority-low">Low</option>
                <option value="priority-neutral">Neutral</option>
            </select>
            <ul>
                <input type="checkbox" id="3pt1" onclick="completeAndDelete(this, 'threePtmade'); displayTaskCompleted();">
                <label for="3pt1">100 left corner 3pt</label>
            </ul>
            <ul>
                <input type="checkbox" id="3pt2" onclick="completeAndDelete(this, 'threePtmade'); displayTaskCompleted();">
                <label for="3pt2">100 upper left side 3pt</label>
            </ul>
            <ul>
                <input type="checkbox" id="3pt3" onclick="completeAndDelete(this, 'threePtmade'); displayTaskCompleted();">
                <label for="3pt3">100 Middle 3pt</label>
            </ul>
            <ul>
                <input type="checkbox" id="3pt4" onclick="completeAndDelete(this, 'threePtmade'); displayTaskCompleted();">
                <label for="3pt4">100 upper right side 3pt</label>
            </ul>
            <ul>
                <input type="checkbox" id="3pt5" onclick="completeAndDelete(this, 'threePtmade'); displayTaskCompleted();">
                <label for="3pt5">100 right corner 3pt</label>
            </ul>
        </details>
    </li>
    <li id="twoPtmade">
        <details>
            <summary>Mid Range Shots: 500 Made<input type="date"></summary>
            <select class="priority-dropdown" onchange="setPriorityColor(this)">
                <option value="priority-high">High</option>
                <option value="priority-medium">Medium</option>
                <option value="priority-low">Low</option>
                <option value="priority-neutral">Neutral</option>
            </select>
            <ul>
                <input type="checkbox" id="2pt1" onclick="completeAndDelete(this, 'twoPtmade'); displayTaskCompleted();">
                <label for="2pt1">100 Left Corner Midrange</label>
            </ul>
            <ul>
                <input type="checkbox" id="2pt2" onclick="completeAndDelete(this, 'twoPtmade'); displayTaskCompleted();">
                <label for="2pt2">100 Upper Left Side Midrange</label>
            </ul>
            <ul>
                <input type="checkbox" id="2pt3" onclick="completeAndDelete(this, 'twoPtmade'); displayTaskCompleted();">
                <label for="2pt3">100 Middle Midrange</label>
            </ul>
            <ul>
                <input type="checkbox" id="2pt4" onclick="completeAndDelete(this, 'twoPtmade'); displayTaskCompleted();">
                <label for="2pt4">100 Upper Right Side Midrange</label>
            </ul>
            <ul>
                <input type="checkbox" id="2pt5" onclick="completeAndDelete(this, 'twoPtmade'); displayTaskCompleted();">
                <label for="2pt5">100 Right Corner Midrange</label>
            </ul>
</ul>
</details>
</li>
<h2>Completed Task</h2>
<ul id="completedTasks"></ul>
<div class="message" id="completionMessage"></div>
<script>
function setPriorityColor(dropdown) {
            const priority = dropdown.value;
            dropdown.parentNode.classList.remove('priority-high', 'priority-medium', 'priority-low');
            dropdown.parentNode.classList.add(priority);
        }
// Function to mark task as complete, trigger celebratory effects, and delete the checkbox
         function completeAndDelete(checkbox, parentTaskId) {
        const listItem = checkbox.parentNode;
        const parentTask = document.getElementById(parentTaskId);

        if (checkbox.checked) {
            // Trigger celebratory animation
            listItem.classList.add('celebration');
            // Move the completed subtask to the completed tasks section
            document.getElementById('completedTasks').appendChild(listItem);

            // Create an "Add back" button
            const addBackButton = document.createElement('button');
            addBackButton.textContent = 'Add Back';
            addBackButton.className = 'addBackButton';
            addBackButton.onclick = function() {
                // Move the subtask back to its original parent task
                parentTask.appendChild(listItem);
                // Remove the "Add back" button
                addBackButton.remove();
            };

            // Append the "Add back" button to the completed subtask
            listItem.appendChild(addBackButton);
        }
    }
        function displayTaskCompleted() {
            const checkboxes = document.querySelectorAll('input[type="checkbox"]');
            let allChecked = true;
            checkboxes.forEach(function(checkbox) {
                if (!checkbox.checked) {
                    allChecked = false;
                }
            });
            if (allChecked) {
                  document.getElementById('completionMessage').textContent = 'All Tasks 100 % Completed';
            }
        }
    </script>
</body>
</html>
