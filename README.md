<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>ClassWork</title>
    <link rel="stylesheet" href="car.css">
    <style>


    </style>
</head>
To Do List
<body>
<ul>

    <li>Cardio: 20 Min Per Machine
        <select class="priority-dropdown" onchange="setPriorityColor(this)">
            <option value="priority-high">High</option>
            <option value="priority-medium">Medium</option>
            <option value="priority-low">Low</option>
        </select>
        <ul>
            <input type="checkbox" id="cardio1" onclick="completeAndDelete(this); displayTaskCompleted();">
            <label for="cardio1">Treadmill</label>
        </ul>
        <ul>
            <input type="checkbox" id="cardio2" onclick="completeAndDelete(this); displayTaskCompleted();">
            <label for="cardio2">Steps</label>
        </ul>
        <ul>
            <input type="checkbox" id="userinput1"onclick="completeAndDelete(this); displayTaskCompleted();">
            <input type="text" name="userinput1"/>
        </ul>


    </li>
    <li>Push Ups: 50 Reps 3 Sets
        <select class="priority-dropdown" onchange="setPriorityColor(this)">
            <option value="priority-high">High</option>
            <option value="priority-medium">Medium</option>
            <option value="priority-low">Low</option>
        </select>
        <ul>

            <input type="checkbox" id="pushup1" onclick="completeAndDelete(this); displayTaskCompleted();">
            <label for="pushup1">Classic</label>
        </ul>
        <ul>
            <input type="checkbox" id="pushup2" onclick="completeAndDelete(this); displayTaskCompleted();">
            <label for="pushup2">Close Grip</label>
        </ul>
        <ul>
            <input type="checkbox" id="userinput2" onclick="completeAndDelete(this); displayTaskCompleted();">
            <input type="text" name="userinput2"/>
        </ul>



    </li>
    <li>3pt Shots: 500 Made<input type="date">
        <select class="priority-dropdown" onchange="setPriorityColor(this)">
            <option value="priority-high">High</option>
            <option value="priority-medium">Medium</option>
            <option value="priority-low">Low</option>
        </select>
    <ul>
        <input type="checkbox" id="3pt1" onclick="completeAndDelete(this); displayTaskCompleted();">
        <label for="3pt1">100 left corner 3pt</label>
    </ul>
    <ul>
        <input type="checkbox" id="3pt2" onclick="completeAndDelete(this); displayTaskCompleted();">
        <label for="3pt2">100 upper left side 3pt</label>
    </ul>
    <ul>
        <input type="checkbox" id="3pt3" onclick="completeAndDelete(this); displayTaskCompleted();">
        <label for="3pt3">100 Middle 3pt</label>
    </ul>
    <ul>
        <input type="checkbox" id="3pt4" onclick="completeAndDelete(this); displayTaskCompleted();">
        <label for="3pt4">100 upper right side 3pt</label>
    </ul>
    <ul>
        <input type="checkbox" id="3pt5" onclick="completeAndDelete(this); displayTaskCompleted();">
        <label for="3pt5">100 right corner 3pt</label>
    </ul>
    </li>
    <li>Mid Range Shots: 500 Made<input type="date">
    <select class="priority-dropdown" onchange="setPriorityColor(this)">
        <option value="priority-high">High</option>
        <option value="priority-medium">Medium</option>
        <option value="priority-low">Low</option>
    </select>
    <ul>
        <input type="checkbox" id="2pt1" onclick="completeAndDelete(this); displayTaskCompleted();">
        <label for="2pt1">100 Left Corner Midrange</label>
    </ul>
    <ul>
        <input type="checkbox" id="2pt2" onclick="completeAndDelete(this); displayTaskCompleted();">
        <label for="2pt2">100 Upper Left Side Midrange</label>
    </ul>
    <ul>
        <input type="checkbox" id="2pt3" onclick="completeAndDelete(this); displayTaskCompleted();">
        <label for="2pt3">100 Middle Midrange</label>
    </ul>
    <ul>
        <input type="checkbox" id="2pt4" onclick="completeAndDelete(this); displayTaskCompleted();">
        <label for="2pt4">100 Upper Right Side Midrange</label>
    </ul>
    <ul>
        <input type="checkbox" id="2pt5" onclick="completeAndDelete(this); displayTaskCompleted();">
        <label for="2pt5">100 Right Corner Midrange</label>
    </ul>
</ul>
</li>
<div class="message" id="completionMessage"></div>
<script>
function setPriorityColor(dropdown) {
            const priority = dropdown.value;
            dropdown.parentNode.classList.remove('priority-high', 'priority-medium', 'priority-low');
            dropdown.parentNode.classList.add(priority);
        }

        // Function to mark task as complete, trigger celebratory effects, and delete the checkbox
        function completeAndDelete(checkbox) {
            if (checkbox.checked) {
                // Trigger celebratory animation
                checkbox.parentNode.classList.add('celebration');
                // Remove the checkbox after a delay
                setTimeout(function() {
                    checkbox.parentNode.remove();
                }, 1000); // Adjust the delay as needed
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
                  document.getElementById('completionMessage').textContent = 'All Tasks Completed';
            }
        }
    </script>
</body>
</html>
