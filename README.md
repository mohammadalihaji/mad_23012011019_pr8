👋 Hello World iOS App in SwiftUI

Aim: Create your first "Hello World" iOS application using the SwiftUI framework.






Course: 2CEIT5PE18: MOBILE APPLICATION DEVELOPMENT.


Submitted By: RAJBHAR PRATHAMKUMAR JAGDISHBHAI, Enrollment number: 23012011026.

🛠️ Project Setup Instructions
Follow these steps to create and configure the basic iOS project in Xcode:


Start a New Project: In Xcode, select File -> New -> Project….


Choose Template: Select the App template from the Application section under the iOS tab.

Configure Project Options:


Product Name: Set the name to hello world.


Interface: Select SwiftUI for the user interface technology.


Language: Set the programming language to Swift.


Options: Ensure that the Core Data and unit testing options are not selected, as they are not needed for this elementary app.


Save Project: Check the Create Git repository on my Mac option and save the project.

📄 Understanding the Code Structure
The project includes two primary source code files:

1. hello_worldApp.swift (Application Entry Point)
This file defines a structure (struct) that acts as the main scene of the app.


A scene handles a group of views.

The code uses WindowGroup to present the main content view, ContentView().

Swift

import SwiftUI

@main
struct hello_worldApp: App {
    var body: some Scene {
        WindowGroup {
            ContentView()
        }
    }
}
2. ContentView.swift (Main View)
This file declares the only view used in the app's main scene.

It displays the text "Hello, world!".

Swift

struct ContentView: View {
    var body: some View {
        Text("Hello, world!")
            .padding()
    }
}
▶️ Running and Previewing the App
Running in the Simulator

Select Simulator: A default iOS simulator (e.g., iPhone 13) is selected at the top of the Xcode window.


Run: Press the Play button at the top left of the project window to build and run the app.



The app will run on the chosen simulator, which provides all the essential features of an actual device for basic testing.



Live Preview (SwiftUI Feature)

Purpose: SwiftUI allows you to preview the app's appearance without running it on a full simulator.






Location: Switch to the ContentView.swift file.


Preview Code Structure: The preview functionality is handled by the ContentView_Previews structure, which conforms to PreviewProvider.



View Updates: Press the Resume button at the top right of the preview window to see updates.


The preview is perfectly synchronized with the code; any changes made in the code editor (left panel) are seen immediately in the preview simulator (right panel)
