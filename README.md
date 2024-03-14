# WT_CW2
this is repository for the app for cw on web technology WIUT

<!-- About the app-> my STUDENT ID 00015991
<!-- The app's purpose is to make it easier for Event managers to manage volunteers. Volunteer
profiles can be made, changed, or deleted by users. They can also read information
about volunteers, which makes volunteer data easy to get to.
This app aims to make managing volunteers easier so that organisations
can do a better job of finding volunteers and coordinating their activities.
the idea of this project come from my own experience in Motorfest2023

some about code
"create.pug" - this file with code stands for the application for and there is very simple and understandble code 
"public" - in this file i added files for img but i thought i would not have much time to do what i wanted so i just let it as it is 

app.get("/edit/:id", (req, res) => {
  const id = req.params.id;

  fs.readFile("./data/students-info.json", (err, data) => {
    if (err) throw err;

    const students = JSON.parse(data);

    const student = students.filter((student) => student.id == id)[0];

    res.render("edit", { student: student });
  });
});

this code defines a web page for editing student information. It reads student data from a file,
finds a specific student by ID, and renders an edit page with the student's data filled in for editing.
This part of the code one of the interesting hard parts of project
->


<!-- Runnig the Application ->
<! -= in order to run the web application there are multiple steps to follow:
1) Run "npm install" in order to install all dependecies.
2) Run "node app" have nodemon in order make it easy to run
<!-- Application dependencies->


<!-- Application dependencies’ list ->
Express.js(nodejs framework) - In order to create the backend of the application
Pug.j5 templete engine for Pug.is makes easy to work with frontend.
nodemon
to work with the application easly while developing it



git hub repository: https://github.com/00015991/WT_CW2



