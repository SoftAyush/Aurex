# Aurex - Personal Money Manager

Aurex is a modern, cross-platform money management application built with **Kotlin Multiplatform** and **Compose Multiplatform**. It allows you to track expenses, manage budgets, and gain insights into your financial health on both Android and iOS from a single codebase.

## 🚀 Features

*   **Expense Tracking:** Easily log and categorize your daily transactions.
*   **Income Management:** Keep track of various income sources.
*   **Budgeting:** Set monthly limits for different categories to stay within your means.
*   **Insights & Analytics:** Visualize your spending habits with intuitive charts (Coming soon).
*   **Cross-Platform Sync:** Consistent experience across Android and iOS devices.

## 🏗 Project Structure

This project follows the Kotlin Multiplatform (KMP) architecture:

*   **[:androidApp](./androidApp)**: The native Android application entry point.
*   **[:iosApp](./iosApp)**: The native iOS application entry point (SwiftUI).
*   **[:sharedLogic](./sharedLogic)**: Contains core business logic, data models, and repository implementations shared between platforms.
    *   [commonMain](./sharedLogic/src/commonMain/kotlin): Core logic used by all targets.
*   **[:sharedUI](./sharedUI)**: Contains the shared UI components and screens built with Compose Multiplatform.
    *   [commonMain](./sharedUI/src/commonMain/kotlin): Shared Compose UI code.

## 🛠 Tech Stack

*   **Kotlin Multiplatform (KMP)**
*   **Compose Multiplatform** (Shared UI)
*   **Kotlin Coroutines & Flow** (Asynchronous programming)
*   **Ktor** (Networking - planned)
*   **SQLDelight** (Local Database - planned)

## 🏃 Running the Apps

You can use the run configurations in Android Studio or use the following commands:

- **Android App:** `./gradlew :androidApp:assembleDebug`
- **iOS App:** Open the [`/iosApp`](./iosApp) directory in Xcode and run it on a simulator or device.

## 🧪 Running Tests

- **Android Tests:** `./gradlew :sharedUI:testAndroidHostTest :sharedLogic:testAndroidHostTest`
- **iOS Tests:** `./gradlew :sharedLogic:iosSimulatorArm64Test`

---
Learn more about [Figma Design](https://www.figma.com/design/xLcF91v80f0FRqGRu7CYqW/Coinpay-Fintech-Finance-Mobile-App-UI-kit--Community---Community-?node-id=4-4&p=f&t=mqTdJq4vYI9S9aDi-0)…


Learn more about [Kotlin Multiplatform](https://www.jetbrains.com/help/kotlin-multiplatform-dev/get-started.html)


