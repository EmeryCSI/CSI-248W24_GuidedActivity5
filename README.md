# Renton Technical College CSI-248
<br />    

![alt text](images/logo.jpg)

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

![alt text](images/1.png)

7. Make sure that your computer and your mobile device are on the same network.
8. Scan this QR Code with the Camera on IOS or using the Expo Go app on Android and you App will launch on your device.

![alt text](images/2.png)

9. Your smartphone screen should now look similar to this:

![alt text](images/3.png)

10. Open up App.js and Change the context of the Text Component to a welcome message. Save the file and notice the changes in both the mobile and web app. Take a screenshot of the Web App and add it the the Screenshots folder.

![alt text](images/4.png)

## Creating our first Native Components

1. Replace the code in App.jsx with the following:

![alt text](images/5.png)

2. We are going to create a button that toggles darkmode for the app.
3. Notice the position of the elements when you run the app. Everything is all the way at the top.
4. We need to style the container that will hold all of our elements.

![alt text](images/6.png)

5. Run the app again and notice that the button has moved to the center of the screen.
6. Let's add the functionality to toggle dark mode.

![alt text](images/7.png)

7. We now have a button which will toggle the isDark state, however we now also need to change the styling of the elements based on that state.
8. If you attempt to access the state directly from the stylesheet you will find that the state is not in scope for the stylesheet.
9. For this reason we must instead access the stylesheel from inside of the component where the state is in scope.

![alt text](images/8.png)

10. Your dark mode button should now be working. Notice that the appearance of the button remains unchanged. Componentd in React Native do not inherit styling the way that they do in HTML/CSS. Also the button component comes with its own styling and is not very customizable. It is the easiest button to use but the least flexible.
11. Take a screenshot of your dark mode on and off and add to the screenshots folder.

## Logging to the Console

1. Lets add another View to get input from the user and log it to the console.
2. Create a new View with a style of logContainer. Inside of that view add a Text with a style of logText and a TextInput with a style of logInput.
3. Create Two buttons with a title of Log to the Console and Warn to the Console.

![alt text](images/9.png)

4. Notice the onChangeText prop for the textInput. This prop takes a callback function which will fire when the text inside of the input changes.
5. It provides a variable to the callback function which contains the text inside of the component.
6. We will call the setInputText function each time this TextInput changes.
7. Lets track the inputText with State.

![alt text](images/10.png)

8. The buttons onPress prop will log the inputText to the console. We have two different ways of logging used here. console.log and console.warn
9. Console.log will appear in your terminal that is running expo.
10. Console.warn will appear in your terminal window but also on the screen of your device.

![alt text](images/11.png)

![alt text](images/12.png)

11. Our dark mode button does not work with our new components. Let's see if we can fix that.
12. Similar to what we did before, if we want to style a component based on a state variable we need to access update the styling from inside of the component.

![alt text](images/13.png)

![alt text](images/14.png)

13. Our Dark mode should be working across all of our components.
14. If you needed a dark/light mode theme beyond just a few components you may want to use a global state container.
15. Take a screenshot of your final functioning app add it to the screenshots folder.
16. `git add .`
17. `git commit -m "Assignment Complete"`
18. `git push`

If you have any questions about this assignment please reach out to myself or our TA for this course. 
https://expo.dev/
