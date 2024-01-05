# React Mock Code Challenge: Plantsy

## Overview

Welcome to the Plantsy app development challenge! In this task, you're going to bring a plant store's admin interface to life. Your mission is to implement key features using React, including state management and interacting with a backend API.

![Demo GIF](https://curriculum-content.s3.amazonaws.com/phase-2/react-hooks-mock-code-challenge-plantshop/plantsy_demo.gif)

## Getting Started

### Initial Setup
1. Run `npm install` in your terminal to install necessary packages.
2. Launch the backend server using `npm run server` on port `6001`.
3. Open a new terminal and start the React app with `npm start`.

### Verify Backend
Before proceeding, check if the backend is running properly by visiting [http://localhost:6001/plants](http://localhost:6001/plants).

## Application Features and API Endpoints

### Core Functionalities
1. **Display All Plants**: Initially, all plants should be displayed.
    - **GET /plants**: Fetches and displays all plant data.

2. **Add a New Plant**: Implement functionality to add a new plant through a form.
    - **POST `/plants`**: Adds a new plant to the list.
    - Required data format:
      ```json
      {
        "name": "string",
        "image": "string",
        "price": number
      }
      ```

3. **Mark Plant as Sold Out**: Allow marking a plant as "sold out".
    - This will be a frontend feature. No specific API endpoint, but think about how to update and render the plant's status in the UI.

4. **Search by Plant Name**: Implement a search feature to filter plants by name.
    - This will primarily be a frontend feature. Utilize the data from the **GET /plants** endpoint for filtering.

### Advanced Features (Optional)
1. **Update Plant Price**: Add functionality to update the price of a plant.
    - **PATCH /plants/:id**: Updates the price of a specific plant.
    - Required data format:
      ```json
      {
        "price": number
      }
      ```

2. **Delete a Plant**: Implement the ability to delete a plant.
    - **DELETE /plants/:id**: Removes a plant from the list.

### Tips for Implementation
- Follow the React component lifecycle for fetching and displaying data.
- Ensure state management is handled efficiently for a dynamic and responsive UI.
- Test each feature as you implement them to ensure functionality.

## Submission
Complete the core deliverables first, and if time permits, tackle the advanced features. Good luck with your coding challenge!
