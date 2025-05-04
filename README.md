
# Postman-demo-repo - GitHub API Integration

## Assignment Overview
This section documents the process of retrieving GitHub user information and creating a new repository using GitHub's API in Postman.

### Part 1: Retrieve User Information from GitHub

1. **Set Up the GET Request:**
   - Set the URL to `{{baseUrl}}user/repos` in Postman.
   - Ensure the Authorization tab is set to **Bearer Token** and input the GitHub personal access token.
   - Execute the GET request to fetch the list of repositories.

2. **Expected Response:**
   - The response should contain a JSON list of repositories.
   
3. **Screenshot:**
   - **Request and Response Setup**: Below is the screenshot of the request setup in Postman and screenshot showing the response containing repository data:
     ![Request and Response Setup](https://github.com/user-attachments/assets/f5622fdf-81b4-4890-9aa0-4462b62248ad)


### Part 2: Create a New Repository

1. **Set Up the POST Request:**
   - Set the URL to `{{baseUrl}}user/repos` in Postman.
   - In the Body section, select **raw** and choose **JSON**.
   - Add the repository data in the following JSON format:
     ```json
     {
       "name": "new-repo-name",
       "description": "Description of the repository",
       "private": false
     }
     ```
   - Replace `new-repo-name` with your preferred repository name.

2. **Expected Response:**
   - The response should confirm the creation of the new repository with details about it.

3. **Screenshot:**
   - **Request and Response Setup**: Below is the screenshot of the request setup in Postman and screenshot showing the response containing repository data:
     ![Request and Response Setup](https://github.com/user-attachments/assets/21cececd-962c-43db-9a55-515112f5e156)

### Conclusion

This document outlines the steps taken to interact with GitHub's API using Postman. The process included retrieving user repository information and creating a new repository using API calls.
