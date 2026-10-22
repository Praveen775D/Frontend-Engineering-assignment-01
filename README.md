# Shipping Bill Management – Frontend Engineering Assignment

## Overview

This project is a React-based Shipping Bill Management application developed as part of a Frontend Engineering Assignment. It provides a user interface to create, save, view, and manage shipping bills.

The implementation focuses on reusable UI components, separation of concerns, form validation, mock services, and a structure that can be connected to a backend API in the future.

## Key Features

- Create and manage shipping bills through a form.
- Reusable components for improved maintainability.
- Form validation for required and domain-specific fields.
- Mock services for simulating asynchronous data operations.
- Save shipping bill details and display saved bills on the dashboard.
- Persist demo data across page refreshes using browser local storage.
- Handle form submission and provide user feedback.
- Download shipping bill data as a flat file.
- Organize business logic, data handling, and UI components separately.

## Technology Stack

- React
- TypeScript
- Vite
- HTML and CSS
- Browser Local Storage
- Asynchronous JavaScript using Promises

## Project Structure

```text
src/
├── shipping-bills/
│   ├── demo-store.ts
│   ├── marks-and-numbers-source.ts
│   ├── model.ts
│   ├── party-dialogs.tsx
│   ├── party-mock-service.ts
│   ├── shipping-bill-form.tsx
│   ├── shipping-bill-service.ts
│   └── workflow.ts
└── index.tsx
```

*Note: This is a simplified view of the project structure.*

### Responsibilities

- **shipping-bill-form.tsx:** Shipping Bill form UI and user interactions.
- **model.ts:** Shipping Bill-related data models and types.
- **shipping-bill-service.ts:** Shipping Bill data operations and service abstraction.
- **party-mock-service.ts:** Mock data operations for party-related options.
- **marks-and-numbers-source.ts:** Source logic for marks and numbers data.
- **demo-store.ts:** Local demo data persistence and synchronization.
- **workflow.ts:** Shipping Bill workflow-related logic.
- **party-dialogs.tsx:** Party-related dialog components.

## Mock Services and API Readiness

The assignment is implemented without requiring a production backend.

Mock service logic is kept separate from the UI so that data operations can be adapted to real API endpoints in the future. Asynchronous operations can simulate network requests and allow the UI to handle loading, success, and error scenarios.

The service layer provides a separation between form interactions and data operations. A future backend integration can replace the mock implementation while preserving the overall UI structure.

**Current limitation:** The application uses demo/local data and does not require a live backend API.

## Validation and Error Handling

The form is designed to validate user input before saving a shipping bill. Validation helps prevent incomplete or invalid submissions and improves the data-entry experience.

The application also provides feedback during form interactions and saving. Additional server-side validation and standardized API error handling can be implemented when a production backend becomes available.

## Data Persistence

The demo implementation uses browser local storage to retain saved shipping bill data across page refreshes.

This approach is intended for frontend demonstration purposes only. Local storage is not a replacement for a production database or server-side persistence.

## Getting Started

### Prerequisites

- Node.js
- npm

### Installation

Clone the repository:

```bash
git clone https://github.com/Praveen775D/Frontend-Engineering-assignment-01.git
cd Frontend-Engineering-assignment-01
```

Install dependencies:

```bash
npm install
```

### Run the development server

```bash
npm run dev
```

Open the local URL displayed in the terminal, typically:

```text
http://localhost:5173/
```

### Build the project

```bash
npx vite build
```

## Verification Performed

The following checks were performed during local testing:

- The application opens in the browser.
- The Shipping Bill form opens and accepts input.
- A Shipping Bill can be saved.
- The saved bill appears on the dashboard.
- Saved demo data remains available after refreshing the page.
- The flat-file download feature works.
- The tested workflow operates without requiring a live backend.

These checks describe the local demo workflow and are not a claim of production or end-to-end backend testing.

## AI Usage and Approach

AI assistance was used as a development aid to understand the existing project structure, plan the refactoring approach, troubleshoot development issues, and improve documentation.

The implementation approach focused on:

1. Understanding the existing Shipping Bill workflow before making changes.
2. Keeping changes focused on the assignment requirements.
3. Separating UI components from data and service logic where practical.
4. Reusing components and existing project dependencies.
5. Using mock data and local persistence because a production backend was unavailable.
6. Running the application and build command to verify the local implementation.
7. Reviewing the limitations of the demo implementation and identifying future improvements.

AI was used to support development and debugging; the final implementation should be reviewed and understood by the developer before submission.

## Limitations and Future Improvements

- Connect the application to a production backend API.
- Add server-side validation and robust API error handling.
- Introduce automated unit and integration tests.
- Improve accessibility and form feedback where needed.
- Replace browser local storage with backend persistence for production use.

## Conclusion

This project demonstrates a frontend approach to Shipping Bill management using React and TypeScript. It emphasizes maintainable component organization, validation, reusable service abstractions, and a functional demo workflow while keeping future backend integration in mind.
