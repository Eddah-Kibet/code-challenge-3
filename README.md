### Blog Post Manager
- This is a client-side blog post manager built using HTML and JavaScript. It allows users to view a list of blog posts, see detailed information for individual posts, and add new posts.

## Features
- Display All Blog Posts:

- Fetches all blog post titles and images from http://localhost:3000/posts on page load.

- Displays post titles as list items (or div elements) within the #post-list section.

## View Post Details:

-Clicking on a post title in #post-list fetches and displays the full details (title, content, author) of that specific post in the #post-detail section.

- Automatically displays the details for the first post as soon as the page loads.

# Add New Blog Post:

- Provides a form (#new-post-form) to input a new post's title, content, and author.

- Adds the new post to the #post-list div upon submission. (Note: This new post does not persist after refreshing the page for this deliverable).

- Simulated Post Deletion: Includes a button to "delete" the main blog post content (client-side only).

# Technologies Used
- HTML: For structuring the web page.

- CSS: For styling (though specific CSS is not provided, it's assumed for visual presentation).

- JavaScript: For all interactive functionalities, including fetching data, handling events, and dynamic DOM manipulation.

### Setup Instructions
- To run this project locally, you will need a simple server to serve the posts data (e.g., using json-server).

- Create your project folder: Create a new directory for your project (e.g., blog-app).

- Save the HTML: Copy your HTML code and save it as index.html inside the blog-app folder.

- Save the JavaScript: Copy your JavaScript code (which will implement the features described above) and save it as index.js inside the blog-app folder.

- Set up a JSON Server (for post data):

- Install Node.js and npm: If you don't have them, download and install Node.js from nodejs.org. npm is included with Node.js.

- Install json-server: Open your terminal or command prompt and run:

 npm install -g json-server

- Create db.json: In your blog-app folder, create a file named db.json with some initial post data

- Start json-server: In your terminal, navigate to your blog-app folder and run:

 json-server --watch db.json --port 3000

- This will start a local server at http://localhost:3000. Your posts data will be available at http://localhost:3000/posts.

- Open index.html in Browser: Once json-server is running, open the index.html file in your web browser.

## Usage
# View All Blog Posts:

- When the page loads, the titles and images of all posts will appear in the "Posts List" section.

# View Individual Post Details:

- Click on any post title in the "Posts List" to display its full content, title, and author in the main blog post area.

- The details for the first post will be displayed automatically on page load.

- Add a New Blog Post:

- Scroll to the "New Post" section.

- Fill in the "Title" and "Content" fields. (The "Author" is pre-filled from HTML).

- Click the "Submit Post" button.

- The new post will be added to the "Posts List".

- Delete Main Post;

- Click the "Delete Post" button in the "New Post" section.

- Confirm the deletion when prompted.

- The main blog post content will be replaced with a "Blog Post Deleted" message.

## Future Enhancements

- Update Post Functionality: Add an "Edit" button to the #post-detail section. When clicked, display an editable form within #post-detail that allows the user to change the post's title and content. Upon form submission, reflect the changes on the frontend (#post-list and #post-detail). No need to persist these changes to the backend for this deliverable.

- Data Persistence: Integrate a real backend (e.g., Firebase, Node.js with Express, Python with Flask/Django) to persist blog posts and comments, so they are not lost on page refresh.

- User Authentication: Implement user login/registration to allow multiple authors and personalized content.

- Rich Text Editor: Integrate a rich text editor for the blog post content input.

- Search and Filtering: Add functionality to search or filter blog posts by title, author, or category.

- Comment Submission: Add a form for users to submit new comments, which are then displayed dynamically and possibly persisted.

- Error Handling: More robust error handling for API requests, form submissions, and data operations.

- Styling and Responsiveness: Add comprehensive CSS to make the blog visually appealing and responsive across various devices.