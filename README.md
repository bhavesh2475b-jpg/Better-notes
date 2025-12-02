# BetterNotes

BetterNotes is a simple, vector-based note-taking application for Android, inspired by Goodnotes. It allows you to create notebooks and draw smooth, vector-based ink notes.

## Features

*   **Notebook Management**: Create multiple notebooks.
*   **Vector Ink Engine**: Smooth drawing experience using Bezier curves.
*   **Tools**: Pen (Black, Red, Blue) and Eraser.
*   **Persistence**: Notes and drawings are automatically saved to your device storage.

## How to Build and Run

Since this project was generated in an environment without a full Android build system, you will need **Android Studio** to build and run the application on your device or emulator.

### Prerequisites

*   **Android Studio** (Hedgehog or newer recommended)
*   **Java Development Kit (JDK) 17** (Usually included with Android Studio)

### Steps

1.  **Download the Code**: Download the source code of this repository.
2.  **Open in Android Studio**:
    *   Launch Android Studio.
    *   Select **Open** (or "Open an existing Android Studio project").
    *   Navigate to the `BetterNotes` folder and select it.
3.  **Sync Gradle**: Android Studio will automatically attempt to sync the project with Gradle files. If it prompts you to download the Android SDK or build tools, click **Yes/Install**.
4.  **Run**:
    *   Connect your Android device via USB (ensure USB Debugging is enabled) OR create an Android Emulator (Virtual Device) via the Device Manager.
    *   Click the green **Run** (Play) button in the toolbar.

### Troubleshooting

*   **SDK Location**: If you get an error about the SDK location, create a `local.properties` file in the `BetterNotes` root directory with the path to your SDK:
    ```properties
    sdk.dir=/Users/YOUR_USER/Library/Android/sdk
    ```
    (On Windows: `sdk.dir=C\:\\Users\\YOUR_USER\\AppData\\Local\\Android\\Sdk`)

## Architecture

*   **Language**: Kotlin
*   **UI**: XML Layouts + Custom Views (`DrawingView`)
*   **Architecture Pattern**: MVVM (Model-View-ViewModel)
*   **Concurrency**: Kotlin Coroutines
*   **Data Format**: JSON (via Gson)
