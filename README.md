# NextJS Starter

- ReactJS vs NextJS
- NextJS is keep getting better and better. 
- It saves so many time
- Big company chooses nextjs
- 

# Requirement
- If you have built reactjs application, state, props, routing, rendering etc, you will be ready to take this course. 
- 

# 0.2 Create a project

- you can add typescript by adding --typescript at the end.
```
npx create-next-app@latest .
```

# 1.0 Library vs Framework

- Whatever you put in the index file will be shown on index.js
- This is the core difference between the framework and the library. 
- Library is what developers call when the time of need. 
- Framework calls your code. 
- In frameork, if you put the code in the right places, it will run the code. 
- Create-react-app starts with the app component. 
- You can choose where to create the routes or components folder in the react. You choose what folder structure to follow.  
- Nextjs has certain rules and nextjs is going to help us. 
- Nextjs abstract some of the reactjs code that we do not need to access. 

- if you create about.js within the pages folder, it will automatically create a route to /about.

# 1.1 Pages

- NextJS calls the code when we put the about.js and index.js in the folder. 
- It is very easy to add the project.
- Thing that matter is the name of the file inside the pages. 
- What doesn't matter is the name of the component. It could be named anything. The name of the component really doesn't matter. 
- you have to export default and pay attention to the name of the file. 
- If the page doesn't exist, it will show the default 404 page from nextjs.
- You don't have to import React when you are exporting the JSX.
- You can just write JSX and it will show up.

# 1.2 Statis Pre Rendering

- One of the best feature is that the page will be pre-rendered or statically generated.
- The difference between create-react-app and nextjs, it will be client-side render. Client-side render means the chrome will do all the work in the rendering of the page. 
- If you look at the source code of the application, you will only see one div, apart, you will see the javascript. 
- Browser get the javascript, and the client-side javascript will build a website. 
- <noscript> is something that the user will see when the javascript is not enabled form the browser. 
- If you are in a slow connection like 3G, if you refresh the page, you will see what will happen. 
- The browser will get the white screen. The brwoser can only build code when the javascript comes. If the user does not have the fast connection, they will see the white screen. 
- If we disable the javascript and refresh the page, it will jsut the same way in the nextjs.
- Source code of the nextjs will have the real HTML. Even if the user has the very slow connection, user will at least see the html. 
- The user will first see the HTML at least and wait for the data to arrive from API. 
- hydration: 
- When you create useState() and the counter, you will get the counter. The source code will have the pre-rendering using the initial state. It will store 0 counter but when the page loads, it will takes over and work the javascript part. 
- This is called hydration basically starting the reactjs in the front end. 
- It will hook into the pre-generated page.
- This is really good for SEO.
- 