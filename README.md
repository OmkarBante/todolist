# To-Do List Fullstack Web App
This is a to-do list web application deployed on Render and powered by MongoDB cloud. It allows users to create and manage multiple to-do lists, add and delete items from those lists, and persist the changes in the cloud database.

## Installation and Usage
The easiest way to use the application is to access the deployed website via https://todolist-cncw.onrender.com/. However, if you prefer to run the app locally, follow these steps:
1. Clone this repository.
2. Install the dependencies by running `npm install` in the root directory. Create a `.env` file in the root directory and set the `mongo_url` environment variable. For example: `mongo_url=<your-mongodb-uri>`
3. Start the server by running npm start or npm run dev in the root directory.
4. Access the web application by opening a browser and navigating to http://localhost:3000/.

## Tools and Libraries Used
The following table lists the tools and libraries used in the development of this web application, along with a brief explanation of why they were chosen.
| Tool/Library | Purpose |
| ----------- | -------- |
| Node.js |	The server-side JavaScript runtime environment used to build the web application. It is popular, well-documented, and provides a robust framework for building web applications. |
| Express.js |	A Node.js web application framework that simplifies the handling of HTTP requests and responses. |
| MongoDB cloud |	A NoSQL database that is easy to scale and well-documented. It was chosen because not much inter-document relationships need to be made for the purposes of this app. |
| Render |	A cloud platform that makes it easy to deploy, manage, and scale web applications. |
| body-parser |	A Node.js middleware used to parse incoming request bodies in a middleware before the request handlers. It helps with requests from the client-side, such as adding and deleting items from the to-do list. |
| dotenv |	A zero-dependency module that loads environment variables from a .env file into process.env. It was used for login security. |
| ejs |	A simple templating engine that allows for the reuse of code, especially when creating new to-do lists. |
| lodash |	A JavaScript utility library that makes string formatting a lot easier. |

## Functionality
When you first access the web application, you are directed to the home page, which is the default to-do list. The title of the to-do list is the date of the day you access the page, and it is prepopulated with three to-do items. However, the items on the to-do list may look different for other users of the web application because they can modify the lists as they wish.

![Screenshot (78)(1)](https://user-images.githubusercontent.com/83286193/225684072-b1166231-41b4-46cd-bca5-0ce4ed5a1eca.png)
### Adding Items to a List
To add an item to a to-do list, simply type the new item name into the last box and then press the "+" button or the Enter key.

### Deleting Items from a List
To delete an item from a to-do list, simply click the checkbox next to the item name.

### Creating New Lists
New to-do lists are created when a new parameter name for a list is inputed into the URL.

### References
- MongoDB's Atlas Cluster Tutorial
- The Coding Train Tutorial on dotenv
- Node.js Gitignore File Template
- Udemy Fullstack Course by Angela Yu
