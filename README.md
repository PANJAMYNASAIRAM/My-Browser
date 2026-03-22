##Project Description

This project is a Wikipedia Search Web App built using JavaScript that allows users to search for topics and view relevant results fetched from an external API.

When a user enters a query and presses Enter, the app retrieves matching Wikipedia articles and displays their title, link, and description dynamically on the webpage.

##Features

🔍 Search Wikipedia articles in real-time

⌨️ Trigger search using Enter key

📡 Fetch data from external API

📄 Displays:
Title (clickable link)

URL
Description
⏳ Loading spinner while fetching data

🔄 Clears previous results before new search

🌐 Opens links in a new tab 

##Technologies Used

HTML5 – Structure (input, results container, spinner)

CSS3 – Styling and layout

JavaScript (ES6) – DOM manipulation, event handling

REST API – Wikipedia search API

Fetch API – For asynchronous data requests 

##Installation Steps

1. Clone the repository git clone https://github.com/PANJAMYNASAIRAM/My-Browser.git
2. Go to project folder "cd My-Browser"
3. Install dependencies "npm install"
4. Start the project "npm start"
   
##Live Demo

https://PANJAMYNASAIRAM.github.io/My-Browser 



##How It Works
User types a query in the search input
Presses Enter key
Spinner is displayed while fetching data
API request is sent using fetch()
Response is converted to JSON
Search results are extracted (search_results)
For each result:
Title, link, and description are created dynamically
Appended to the results container
Spinner is hidden after results are displayed
📷 Output

Each result shows:

🔗 Clickable title
🌐 URL link
📝 Short description
🔧 Future Enhancements
🔎 Add search button (not just Enter key)
❌ Handle API errors (network issues)
📱 Improve mobile responsiveness
⭐ Add “Save Favorite Results”
🎨 Enhance UI with cards and animations
🚀 Use Cases
Quick information lookup 🌐
Learning API integration
Real-time search applications
Portfolio project for beginners
💡 Bonus Improvement (Optional Upgrade)

Use debouncing to avoid too many API calls while typing:

let timerId;
searchInputEl.addEventListener("input", function(event) {
    clearTimeout(timerId);
    timerId = setTimeout(() => {
        searchWikipedia({ key: "Enter" });
    }, 500);
}); 






