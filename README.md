# feb-2025-avasjcript-events-and-basic-interactivity

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>JavaScript Events Example</title>
  <style>
    #message {
      display: none;
      margin-top: 10px;
      padding: 10px;
      background-color: lightblue;
      border: 1px solid blue;
      border-radius: 5px;
    }
  </style>
</head>
<body>
  <h1>JavaScript Events and Interactivity</h1>
  
  <button id="toggleButton">Show Message</button>
  <div id="message">Hello! This is a toggleable message.</div>

  <script>
    // Select the button and the message element
    const toggleButton = document.getElementById("toggleButton");
    const message = document.getElementById("message");

    // Add a click event listener to the button
    toggleButton.addEventListener("click", function () {
      if (message.style.display === "none") {
        // Show the message and change the button text
        message.style.display = "block";
        toggleButton.textContent = "Hide Message";
      } else {
        // Hide the message and change the button text
        message.style.display = "none";
        toggleButton.textContent = "Show Message";
      }
    });
  </script>
</body>
</html>
