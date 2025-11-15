# PlayGround

## Overview

PlayGround is an Android application developed in **Kotlin**, designed
as a modular and extensible environment for experimenting with UI
components, state handling, navigation, and interaction patterns. The
project is organized following a lightweight **MVC
(Model--View--Controller)** architecture complemented by a shared kernel
for cross-cutting concerns.

The application demonstrates clean architectural separation,
command-based interactions, and centralized state management, providing
a clear and maintainable structure for scalability and experimentation.

## Technology Stack

-   **Language:** Kotlin\
-   **Platform:** Android (AndroidX)\
-   **Build System:** Gradle (Kotlin DSL)\
-   **UI Toolkit:** Android Views\
-   **Architecture:** MVC + Shared Kernel\
-   **Design Patterns:** Command Pattern, Singleton, Router Pattern

## Project Structure

    PlayGround/
     └── app/
          └── src/main/java/com/pamn/playground
               ├── controller
               ├── model
               ├── view
               └── sharedKernel

## Architectural Overview (MVC)

### Model

Contains domain entities and application state structures.

Main components: - Counter -- Domain model representing a simple
counter. - Media -- Entity for managing media items. - AppState --
Central state object.

### View

UI components responsible for rendering the current AppState and
emitting UI events.

### Controller

Coordinates interactions between Views and the Model using Commands.

## Shared Kernel

Cross‑cutting services such as: - AppStateStore - HistoryStore - Router

## Design Patterns Used

-   Command Pattern
-   Router Pattern
-   Singleton

## Features

-   Counter operations
-   Media selection
-   Undo support
-   Modular MVC structure

## Build

    ./gradlew build

## Run

Open the project in Android Studio and run on an emulator or device.
