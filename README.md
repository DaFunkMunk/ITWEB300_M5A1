JavaScript API Example: Geolocation API

The Geolocation API is a built-in JavaScript API that allows web applications to access the geographical location of a user, like the food truck example shown during class. This can be 
extremely useful for a variety of web-based services, such as location-aware apps (e.g., weather apps, local restaurant finders, mapping tools), allowing them to provide personalized 
experiences based on the user's current position. The API uses device hardware such as GPS, Wi-Fi, or IP address location data to determine where the user is located.

The API is accessed through the navigator.geolocation object and provides methods such as getCurrentPosition() and watchPosition(). getCurrentPosition() retrieves the device's current 
position, while watchPosition() continuously monitors the position and updates it as the device moves. A callback function is used to process the position data once it’s available, and 
optional error handling can be implemented to manage user denial or technical issues.

Example:
if ("geolocation" in navigator) {
  navigator.geolocation.getCurrentPosition(
    function (position) {
      console.log("Latitude:", position.coords.latitude);
      console.log("Longitude:", position.coords.longitude);
    },
    function (error) {
      console.error("Error getting location:", error.message);
    }
  );
} else {
  console.log("Geolocation is not supported by this browser.");
}

Challenges:

Working on this assignment was both informative and practical. It provided the opportunity to work hands-on with jQuery, AJAX, and dynamic data handling using JavaScript. Implementing 
features like form submission, dynamic ticket listing, and real-time lookups helped reinforce my understanding of how front-end code can communicate with backend services, even when 
using simulated or in-memory data.

One challenge was getting AJAX POST requests to behave correctly without a real backend endpoint. To solve this, I implemented temporary in-memory storage using JavaScript arrays and 
functions to mimic server behavior. Another tricky part was preserving the display of all submitted tickets while supporting specific lookups. Overall, this assignment improved my 
skills with JavaScript events, DOM manipulation, and user interface logic.



