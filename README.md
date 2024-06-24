# GitHub User Search and Profile Display

This project is a web application that allows users to search for GitHub usernames and view detailed information about the users, including their followers, following, public repositories, and a list of their repositories. The application is built using Angular and leverages Bootstrap for styling and Material Icons for additional UI elements.

## Key Features

- **Search GitHub Users**: Users can search for GitHub usernames using an input form.
- **User Profile Display**: Displays the user's profile information including avatar, name, bio, followers, following, and public repositories.
- **Repository Showcase**: Lists the user's repositories with basic information such as repository name and description.
- **Pagination**: Handles pagination for user repositories if the number of repositories exceeds the page limit.
- **Skeleton Loader**: Displays a skeleton loader while fetching data from the GitHub API.

## Application Structure

- **Main Component**: The main Angular component `<app-root>` serves as the entry point of the application.
- **Form and Input Handling**: A form is used to capture the GitHub username and trigger the search action.
- **User Profile Card**: Displays a card with user details such as avatar, name, bio, followers, following, and public repositories.
- **Repository List**: Shows a list of the user's repositories in a grid layout.
- **Pagination**: Utilizes Angular Material's paginator to handle pagination of repositories.

## Code Breakdown

### HTML Structure

- **Bootstrap and Material Icons**: The application includes Bootstrap for responsive design and Material Icons for icons.
- **Form**: A form with an input field and a search button to capture the GitHub username.
- **User Profile Card**: Conditional rendering of the user's profile details or an error message based on the search result.
- **Skeleton Loader**: Provides visual feedback during data fetching.

### Angular Component Methods

- **searchUser(userName, limit)**: Handles the form submission to search for the specified GitHub username. It accepts `userName` and `limit` as parameters.
- **checkUserDetailsMethod()**: Toggles the view between the user profile summary and detailed user information.
- **getRepos(event, initialLoad)**: Handles pagination and fetches the user repositories based on the current page and page size.

## Usage

1. **Search for a User**: Enter a GitHub username in the search input field and click the "Search" button.
2. **View User Details**: If the user exists, their profile details will be displayed. Click "See Details" to view more information.
3. **Pagination**: If the user has many repositories, use the paginator at the bottom to navigate through the repositories.

## Project Setup and Execution

1. **Clone the Repository**:

    ```bash
    git clone https://github.com/hemanthgithub642/angular_task
    cd your-repo
    ```

2. **Install Dependencies**:

    ```bash
    npm install
    ```

3. **Run the Application**:

    ```bash
    ng serve
    ```

    The application will be available at `http://localhost:4200`.

## Technologies Used

- **Angular**: Framework for building the front-end application.
- **Bootstrap**: For responsive design and styling.
- **Material Icons**: For icons used in the UI.
- **GitHub API**: To fetch user data and repositories.

## Conclusion

This application provides an intuitive interface for searching GitHub users and viewing their profile details. It makes use of Angular for robust front-end development and Bootstrap for modern, responsive design. The integration with the GitHub API allows for real-time fetching and display of user data.
