# Critical-Mass-Internship-Tasks

## Work / Project Examples

### Project 1: RTA Learning Tool

URL: https://zen-roentgen-b5c232.netlify.com/ 

Github Source Code: https://github.com/hassanfarahani/RTA-Learning-Tool

I am working part time (remote) for Saga Company helping them to develop some petroleum-learning tool. They have many petroleum-engineering instructors to teach petroleum-engineering concepts, and my role is to develop an interactive learning tool using Vue.js and D3.js. I am still working on RTA learning tool to improve its appearance, and functionalities, but I developed it by myself because Saga is a small start-up company. They do not have many developers. I learned D3.js during this project, and how combine vue & d3.


### Project 2: WMS Application 

URL: https://wms-app.netlify.com

Github Source Code: https://github.com/hassanfarahani/WMS

This is a simple Well Management System (WMS) application (personal project). I was fetching the well data from an API, and displaying them on the screen, but first user need to sign in in order to access the well data. If user do not have an account, he/she should first sign up, and then sign in to edit (add, edit and delete) the well data. Without sign in, user can just observe the list of the wells. Unfortunately, the API I was fetching the well data from, is not working anymore, but you can check the source code to see how I have used this API. The reason I put this project in my list to show it to you is that I learned a lot from this project.


### Project 3: Chat Application 

URL: https://inspiring-mcnulty-f3d6e2.netlify.com/

Github Source Code: https://github.com/hassanfarahani/Chat-App

I had an interview with Cisco Company (They were looking for Intermediate UI Developer). They wanted me to build a simple chat application. I built this application using Vue.js, and Vuex.

 
## Inspiration

### Work Example 1: RTA Learning Tool

This is a very inspiring project for me, because 
1.	I learned how to combine vue.js and d3.js (there is not many source on the internet to teach how to use these two together, I figured it out by myself). 
2.	I learned mounted () hook in vue.js, and when we need it because in my entire previous vue.js projects, I have always been using the created () hook, and I did not know that when we needed to use mounted () hook in an application. In this project, I needed to add a SVG element to the DOM in order to show the different graphs, and to do this, I needed to use mounted () hook (instead of created () hook) because mounted () hook is called after DOM has been mounted so you can access DOM elements and add SVG element to the DOM.
3.	I learned when I needed to use watcher in vuejs because in this application, I had an array (a computed property containing the data for each graph like this: [[…], […], …]). What I wanted was that when the content of this array changed (when user add a new graph to the current graphs by changing the sliders), those vue components responsible for generating the graphs using this array, should automatically rerendered in order to display the new added graph. This did not happened (rerendering) because vuejs (computed property) do not know that the content of the array has been changed. To make vuejs aware of this array content change, I used a watcher for this computed property so that whenever user change the content of the array, vuejs rerender those components. 
4.	I learned how to define routes using route parameters. In this application, I needed to use two vue components for different routes (different lessons). First I tried to hardcode the routes for each lesson (path: “/lesson-1/production-plot” & path: “/lesson-2/production-plot”), but I got the following error in my console: duplicate named routes. The reason of this error was that I had used two vue components (production-plot & rta-plot) for all my routes. To resolve this issue, I passed a dynamic parameter to a single path (path: “/:lessonId/production-plot”), then I retrieved this parameter from the route in the vue component, and used that parameter to change the vue component for that route.



### Work Example 2: WMS Application

Making this application was a very good opportunity for me to learn authentication:
1.	I learned what is token and how to use it in order to authenticate the user. I learned how to get token from the response of the post request (which has been sent to the server after user inputs its username, and password), and store it in the state. 
2.	I figured it out that in order to give user the ability to reload the page after sign in, I need to store the token in the local storage.
3.	I learned how to create protected guards for a route by checking if the user is signed in or not.

 
## Focus

If I were given the time and resource to learn something, I would prefer to continue learning React.js (Udemy course), and then starting a real project using React.js, and Redux. The reason is that I have not had time to build an application using React.js yet; in fact, in all of my projects, I have used vue.js. Based on my understanding, React.js is the most popular framework in the industry. 

## Code Challenge
Link to my solution: https://codesandbox.io/s/2020-internship-exercise-menu-su3ph
