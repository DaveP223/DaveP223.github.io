<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>ClassWork</title>
       <link rel="stylesheet" href="car.css">
    <style>
    
    </style>
</head>
<h1>To Do List</h1>
<div class="message" id="completionMessage"></div>
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
                <button class="deleteButton" onclick="deleteSubtask(this)">Delete</button>
            </ul>
            <ul>
                <input type="checkbox" id="cardio2" onclick="completeAndDelete(this, 'cardioTask'); displayTaskCompleted();">
                <label for="cardio2">Steps</label>
                <button class="deleteButton" onclick="deleteSubtask(this)">Delete</button>
            </ul>
            <ul>
                <input type="checkbox" id="userinput1"onclick="completeAndDelete(this, 'cardioTask'); displayTaskCompleted();">
                <input type="text" name="userinput1"/>
                <button class="deleteButton" onclick="deleteSubtask(this)">Delete</button>
            </ul>
        </details>
<button class="deleteButton" onclick="deleteSubtask(this)">Delete</button>
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
                <button class="deleteButton" onclick="deleteSubtask(this)">Delete</button>
            </ul>
            <ul>
                <input type="checkbox" id="pushup2" onclick="completeAndDelete(this, 'pushupsTask'); displayTaskCompleted();">
                <label for="pushup2">Close Grip</label>
                <button class="deleteButton" onclick="deleteSubtask(this)">Delete</button>
            </ul>
            <ul>
                <input type="checkbox" id="userinput2" onclick="completeAndDelete(this, 'pushupsTask'); displayTaskCompleted();">
                <input type="text" name="userinput2"/>
                <button class="deleteButton" onclick="deleteSubtask(this)">Delete</button>
            </ul>

        </details>
<button class="deleteButton" onclick="deleteSubtask(this)">Delete</button>
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
                <button class="deleteButton" onclick="deleteSubtask(this)">Delete</button>
            </ul>
            <ul>
                <input type="checkbox" id="3pt2" onclick="completeAndDelete(this, 'threePtmade'); displayTaskCompleted();">
                <label for="3pt2">100 upper left side 3pt</label>
                <button class="deleteButton" onclick="deleteSubtask(this)">Delete</button>
            </ul>
            <ul>
                <input type="checkbox" id="3pt3" onclick="completeAndDelete(this, 'threePtmade'); displayTaskCompleted();">
                <label for="3pt3">100 Middle 3pt</label>
                <button class="deleteButton" onclick="deleteSubtask(this)">Delete</button>
            </ul>
            <ul>
                <input type="checkbox" id="3pt4" onclick="completeAndDelete(this, 'threePtmade'); displayTaskCompleted();">
                <label for="3pt4">100 upper right side 3pt</label>
                <button class="deleteButton" onclick="deleteSubtask(this)">Delete</button>
            </ul>
            <ul>
                <input type="checkbox" id="3pt5" onclick="completeAndDelete(this, 'threePtmade'); displayTaskCompleted();">
                <label for="3pt5">100 right corner 3pt</label>
                <button class="deleteButton" onclick="deleteSubtask(this)">Delete</button>
            </ul>
        </details>
        <button class="deleteButton" onclick="deleteSubtask(this)">Delete</button>
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
                <button class="deleteButton" onclick="deleteSubtask(this)">Delete</button>
            </ul>
            <ul>
                <input type="checkbox" id="2pt2" onclick="completeAndDelete(this, 'twoPtmade'); displayTaskCompleted();">
                <label for="2pt2">100 Upper Left Side Midrange</label>
                <button class="deleteButton" onclick="deleteSubtask(this)">Delete</button>
            </ul>
            <ul>
                <input type="checkbox" id="2pt3" onclick="completeAndDelete(this, 'twoPtmade'); displayTaskCompleted();">
                <label for="2pt3">100 Middle Midrange</label>
                <button class="deleteButton" onclick="deleteSubtask(this)">Delete</button>
            </ul>
            <ul>
                <input type="checkbox" id="2pt4" onclick="completeAndDelete(this, 'twoPtmade'); displayTaskCompleted();">
                <label for="2pt4">100 Upper Right Side Midrange</label>
                <button class="deleteButton" onclick="deleteSubtask(this)">Delete</button>
            </ul>
            <ul>
                <input type="checkbox" id="2pt5" onclick="completeAndDelete(this, 'twoPtmade'); displayTaskCompleted();">
                <label for="2pt5">100 Right Corner Midrange</label>
                <button class="deleteButton" onclick="deleteSubtask(this)">Delete</button>
            </ul>
            
</details>

<button class="deleteButton" onclick="deleteSubtask(this)">Delete</button>
</li>
</ul>
<h2>Completed Task</h2>
<ul id="completedTasks"></ul>
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
            // Triggering celebratory animation
            listItem.classList.add('celebration');
            // Moving the completed subtask to the completed tasks section
            document.getElementById('completedTasks').appendChild(listItem);

            // Creating an "Add back" button
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
         function deleteSubtask(button) {
        const listItem = button.parentNode;
        listItem.remove();
    }
    </script>
</body>
</html>
