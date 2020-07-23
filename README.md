#### Project Description

The goal of this project is to have a pre-test on candidates' React and Redux skills. We understand that you might be on a tight schedule, so we do not aim for a perfect completion of this web project. Instead, we see this as a quick check on the basic concepts of web programming and help us to better understand your strengths. During your progress, if needed, feel free to consult with `Gabriel` regarding any issues or ideas related to the project.

You will be implementing a React version of to-do list web app, in which the user could easily add a todo/goal, delete a todo/goal or mark a todo/goal as completed. We have provided all the UI components, the actions creator and some of the middleware (for example: logger). The only missing parts of this web app is the:

* handle function to dispatch
* reducer functions * 2
* initialization of store and its binding with all middleware

`The starter code is in the URL: https://github.com/asalpha/react-todo-example/blob/master/index.html`

<i> Note that for easier understanding, we have embedded the React with basic HTML all in one file. You are not required to separate them but can just work on this one file code. All the missing functions are marked as `TO IMPLEMENT`</i>

#### Estimated Time To Complete

We have provided hints(even pseudocode) on all of the functions you need to implement. We have also handled the initial data flow as well as how the data being rendered from store. The estimated time to finish this project (after understand the code) will be around 30min to 60min.

#### Submission

The candidate is required to first fork the repository and start work from their. Upon completion, please either zip the code or send the URL to your public forked repository to `Gabriel` (Email: gabriel@manorlead.com, Wechat: ruozhenruozhen). 

Please note, if you only completed `todo` part, we consider it as a full mark as well. Completing both will mark as extra bonus and assets.

The due date for submission is on Monday 8pm (July 27th, 2020 EST). We recommend you sending all the progresses by due regardless of whether the app is fully completed. 

#### Run Enviroment:

1. Clone the project
2. `cd` into the project directory where project lives
3. Install dependencies: `npm install`
4. Start the app: `npm start`

<i>Report any error directly to `Gabriel`</i>

##### Code Explanation - `Must Read`

For line 9:

> Line 9 includes a faked backend server code. Please free to place its URL in the browser and see the functions provided. You will be making Promise-based API call for dispatch functions from line 71-94. We have provided enough hint on which method you will be calling for each dispatch function. So going through more details on those backend function is not recommended. 

For line 21 - 26 & line 28-69

> Those will be all the actions you will interact with. You do not need to create any new actions to complete this App.
>
> line 28-29 are all the action creator. Hint: `todos, goals, loading` are data stored in the redux-store

For line 71-94

> To be implemented to call the dispatch function. Note that you must use `Thunk` in order to call API function here.
>
> Hint: We are using an optimistic updates here which means that the UI is updated first before the API is making called (if later API is failed, you will update the UI back to origin). To do so, inside of handler function, you should first try to dispatch appropriate actions. And then call the API functions and try to catch if there is any error occurs. If so, you will need to dispatch back and maybe alert the user that an error has happen. `alert('An error occured')` . 
>
> Extra Hint: check line 96-105 which is a handle function to run initially when app is rendered.

For line 107-136:

> This parts are the reducer function you need to implement. For each line marked as `TO IMPLEMENT` , you will write a one line code to update the state parameter accordingly. 
>
> Hint: check line 137-144 which is a reducer function to check if the app is loading.

For line 146-171:

> They are 2 of 3 middleware we have provided for you. You need to understand them which we might ask during interview process.

#### Interview Process - `Read after completion of project`

We appreciate your interests on our company, and we will be looking forward to having an interview process after check the project submissions. We value your experience and that's why we have spend efforts on  making this project to have a overall views on your strengths and skills. The interview process will happen in the same week as the due date of this project. You could expect an update before Wednesday 3pm. 

During the interview process, we will formally introduce ourselves and our company missions and then we can go over your resume as well as some of the basic frontend questions. Specifically, you could expect the following questions:

* Middleware: how Thunk, Logger, Check middleware has been applied in to-do app? What's the use cases?
* How to convert this code into `react-hook` instead?
* React lifecycle vs. hook lifecycle.

----

© 2020 Manorlead

contact: gabriel@manorlead.com

<img src="C:\Users\gugab\AppData\Roaming\Typora\typora-user-images\image-20200723150823106.png" alt="image-20200723150823106" style="zoom:25%;margin-left:0" />
