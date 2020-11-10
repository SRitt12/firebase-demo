# Firebase Demo
This is a demo of developing web apps using the Hosting, Authentication, and Storage features of Firebase.

## Prerequisites:
* Initialized Firebase project
* Node/NPM
* VS Code or text editor

## Process:

 ### Hosting
 
1. Create and initialize a Firebase project with hosting, auth, and storage components selected
2. After initializing, go to https://firebase.google.com/docs/hosting/quickstart and follow the steps there to set up the project for hosting
3. Deploy the hosted project and verify it is working correctly

  ### Authentication
  
4. Watch the Firecast video [Using FirebaseUI Auth, on the Web](https://www.youtube.com/watch?v=hb85pYZSJaI&t); you can also go to https://firebase.google.com/docs/auth/web/firebaseui and follow the instructions there, but the video will get you set up and ready to go much faster. I personally found the Firecasts to be much more clear and informative than the documentation in general, so I would recommend them over the documentation whenever there is a video about the topic you need.
5. Follow along with the steps of your chosen guide to get the authentication and ui set up. Make sure to add whichever auth methods you would like to have for your site. If you follow the video and get the boilerplate code from github, you can just uncomment whichever methods you want.
6. If you haven't already, make sure to make a second html page and set that as the `signInSuccessUrl`
7. Go to your hosted site and verify that you can log in and are sent to the page you set for `signInSuccessUrl`

  ### Storage
8. Watch the Firecast [Getting Started with Firebase Storage on the Web](https://www.youtube.com/watch?v=SpxHVrpfGgU&t). Again, you can also read the docs at https://firebase.google.com/docs/storage/web/start, but the Firecast is easier.
9. Follow along the instructions to create your file input object and progress bar (The progress bar is totally optional, I just like it).
10. Add the given JavaScript code to the input and progress bar.
11. At this point you have a functional upload system, however I also created a dynamic list that shows what files have been uploaded. To do this, first create an unordered list in html with an `id` and no list items. I named mine `itemlist`.
12. Inside the event listener for the file upload write JavaScript code to create a variable referencing `itemlist` and a variable referencing a new `li` element.

        var list = document.getElementById("itemlist");
        var entry = document.createElement('li');
13. Add the text of the uploaded files name to the `li` you just created, and add the entry to `itemlist`. 

        entry.appendChild(document.createTextNode(file.name));
        list.appendChild(entry);
14. You should now have an unordered list that updates with a new item every time a file is uploaded.


## Project Code
https://github.com/SRitt12/firebase-demo/tree/master/public

## References Used
   [Firebase Documentation](https://firebase.google.com/docs/)
   
   [The Firebase YouTube Channel](https://www.youtube.com/c/firebase), specifically the [Firecasts](https://www.youtube.com/playlist?list=PLl-K7zZEsYLnJVX_0zbKytptZGugPIbJR)
   
   https://www.w3schools.com
   
## Demo Video
https://app.vidgrid.com/view/PoEL5ONhLPXe
   
