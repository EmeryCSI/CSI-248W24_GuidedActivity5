# Renton Technical College CSI-248
<br />    

<div align="center">  
    <img src="logo.jpg" alt="Logo">
    <h3 align="center">Guided Activity 5</h3>
</div>

This repository is a part of CSI-248 at Renton Technical College.

## Guided Activity 5 - If the images are not loading use the word doc in this repository GA5_instructions.docx

## Setup Expo - If you have already done this in class you may skip this step

1. Sign up for an account at https://expo.dev/
2. Install Expo Go on your mobile device in the Apple App Store or Google Play Store
3. Sign in to the Expo Go App using your account you made at expo.dev

## Clone the repo

1. Clone the repository to your local machine. (Do not use OneDrive for assignments in this course!)
2. Make note of the folder where you cloned the repository.
3. After you have cloned this repository navigate to your local repository using the cd command.
4. Open the repository in Visual Studio Code by typing `code .`
5. Create a folder to store the requested Screenshots for this assignment.

## Creating your first react-native project
1. Open the terminal in Visual Studio Code and create a new expo app by running `npx create-expo-app my-first-app`
2. Run `cd my-first-app`
3. You are now in the root project of the folder. Notice that there are some files that look familiar such as package.json and App.js
4. Run `npx expo install react-dom react-native-web @expo/webpack-config` to enable react-native for web
5. Run `npx expo start` to launch the project. You will see a QR Code in the terminal.
6. Type `w` to launch the app in a web browser. You should now see your app running in your default browser.
7. You can use the web browser for the screenshots.

![Screenshot 2023-10-25 at 1 58 40 PM](https://github.com/EmeryCSI/csi248-guidedactivity5/assets/102991550/644981f9-4950-480a-a180-e6e793f5cb7d)

7. Make sure that your computer and your mobile device are on the same network.
8. Scan this QR Code with the Camera on IOS or using the Expo Go app on Android and you App will launch on your device.

![Screenshot 2023-10-25 at 1 47 54 PM](https://github.com/EmeryCSI/csi248-guidedactivity5/assets/102991550/2d808d8f-1811-4456-b857-c332d6dcb6cb)

9. Your smartphone screen should now look similar to this:

![Screenshot 2023-10-25 at 1 49 42 PM](https://github.com/EmeryCSI/csi248-guidedactivity5/assets/102991550/aaf0a383-5342-4e69-9cd7-494afd2d71de)

10. Open up App.js and Change the context of the Text Component to a welcome message. Save the file and notice the changes in both the mobile and web app. Take a screenshot of the Web App and add it the the Screenshots folder.


![Screenshot 2023-10-25 at 2 01 14 PM](https://github.com/EmeryCSI/csi248-guidedactivity5/assets/102991550/1800cfbc-1e87-4295-972a-a4254a70c89c)


## Creating our first Native Components

1. Replace the code in App.jsx with the following:

![Screenshot 2023-10-30 at 5 34 03 AM](https://github.com/EmeryCSI/csi248-guidedactivity5/assets/102991550/e1b7bb60-c25a-4db3-94e7-7bce187b6471)


2. We are going to create a button that toggles darkmode for the app.
3. Notice the position of the elements when you run the app. Everything is all the way at the top.
4. We need to style the container that will hold all of our elements.

![Screenshot 2023-10-30 at 5 37 03 AM](https://github.com/EmeryCSI/csi248-guidedactivity5/assets/102991550/dd8f6486-068c-4455-be29-38938b236272)

5. Run the app again and notice that the button has moved to the center of the screen.
6. Let's add the functionality to toggle dark mode.

![Screenshot 2023-10-30 at 5 43 17 AM](https://github.com/EmeryCSI/csi248-guidedactivity5/assets/102991550/d07d7442-2421-4e85-9d5a-109b3a8546d2)

7. We now have a button which will toggle the isDark state, however we now also need to change the styling of the elements based on that state.
8. If you attempt to access the state directly from the stylesheet you will find that the state is not in scope for the stylesheet.
9. For this reason we must instead access the stylesheel from inside of the component where the state is in scope.

![Screenshot 2023-10-30 at 5 47 31 AM](https://github.com/EmeryCSI/csi248-guidedactivity5/assets/102991550/5404b8fd-5917-498e-b754-731fab1e499a)

10. Your dark mode button should now be working. Notice that the appearance of the button remains unchanged. Componentd in React Native do not inherit styling the way that they do in HTML/CSS. Also the button component comes with its own styling and is not very customizable. It is the easiest button to use but the least flexible.
11. Take a screenshot of your dark mode on and off and add to the screenshots folder.

## Logging to the Console

1. Lets add another View to get input from the user and log it to the console.
2. Create a new View with a style of logContainer. Inside of that view add a Text with a style of logText and a TextInput with a style of logInput.
3. Create Two buttons with a title of Log to the Console and Warn to the Console.

![Screenshot 2023-10-30 at 5 53 11 AM](https://github.com/EmeryCSI/csi248-guidedactivity5/assets/102991550/c8e5accc-abaf-4519-906f-b43e5376db78)

4. Notice the onChangeText prop for the textInput. This prop takes a callback function which will fire when the text inside of the input changes.
5. It provides a variable to the callback function which contains the text inside of the component.
6. We will call the setInputText function each time this TextInput changes.
7. Lets track the inputText with State.

![Screenshot 2023-10-30 at 5 57 36 AM](https://github.com/EmeryCSI/csi248-guidedactivity5/assets/102991550/69cee612-c6bd-4138-9659-136aee0c01f8)

8. The buttons onPress prop will log the inputText to the console. We have two different ways of logging used here. console.log and console.warn
9. Console.log will appear in your terminal that is running expo.
10. Console.warn will appear in your terminal window but also on the screen of your device.

![Screenshot 2023-10-30 at 6 01 46 AM](https://github.com/EmeryCSI/csi248-guidedactivity5/assets/102991550/353d2b59-b070-4cb8-9b77-b2f866ebd22b)

![Screenshot 2023-10-30 at 6 01 56 AM](https://github.com/EmeryCSI/csi248-guidedactivity5/assets/102991550/a9222c84-ca31-4b6e-b158-1c23c8bc863e)

11. Our dark mode button does not work with our new components. Let's see if we can fix that.
12. Similar to what we did before, if we want to style a component based on a state variable we need to access update the styling from inside of the component.

![Screenshot 2023-10-30 at 6 07 18 AM](https://github.com/EmeryCSI/csi248-guidedactivity5/assets/102991550/11f1fa2d-16ce-43ed-a72a-bdbdfb82d882)


![Screenshot 2023-10-30 at 6 07 56 AM](https://github.com/EmeryCSI/csi248-guidedactivity5/assets/102991550/52ef1062-1fae-4145-b04b-e75d37145ad8)

13. Our Dark mode should be working across all of our components.
14. If you needed a dark/light mode theme beyond just a few components you may want to use a global state container.
15. Take a screenshot of your final functioning app add it to the screenshots folder.
16. `git add .`
17. `git commit -m "Assignment Complete"`
18. `git push`

If you have any questions about this assignment please reach out to myself or our TA for this course. 
https://expo.dev/
