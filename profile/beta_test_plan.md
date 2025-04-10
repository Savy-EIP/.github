### **BETA TEST PLAN – Savy**

## **1. Core Functionalities for Beta Version**

| **Feature Name**               | **Description**                                                                                                 | **Priority (High/Medium/Low)** | **Changes Since Tech3**      |
| ------------------------------ | --------------------------------------------------------------------------------------------------------------- | ------------------------------ | ---------------------------- |
| Send messages                  | User sends a message to an Echo with a dedicated interface                                                      | High                           |                              |
| Receive messages               | User receives a response to the message they sent                                                               | High                           |                              |
| Messages history               | User can see the message history in a conversation                                                              | High                           |                              |
| Diversity of Echoes            | User has access to many differents Echoes                                                                       | High                           | Feature's name change        |
| Chat Page                      | User uses this page to chat with an Echo                                                                        | High                           |                              |
| Discussion List Page           | The list of all available discussions where the user can choose                                                 | High                           |                              |
| Discussion Page                | The main page of the discussion where the user can see their recent chats, 3 random topics, and 3 random places | High                           |                              |
| Sign In / Sign Up Page w/o SSO | User can sign in or create an account with their email and password                                             | High                           | Split the w/ SSO and w/o SSO |
| Navigation Bar                 | User can navigate through Home/Discussion/Stats/Lessons page                                                    | Medium                         |                              |
| Top Bar                        | User can switch languages to learn and view their profile                                                       | Medium                         |                              |
| See Errors on Messages         | User can see errors on messages when sending one                                                                | Medium                         | Added more precisions        |
| Discuss w/ Savy on an error    | User can start a discussion with Savy to speak about an error to understand it                                  | Medium                         | Added for better UX          |
| Profile Page                   | User can view and edit their profile information, change the language of the app and access some settings       | Medium                         |                              |
| Lessons Page                   | User can access and view basics lessons on the language they are learning                                       | Low                            |                              |
| Moderation Savy                | The AI Savy moderates the messages between the user and the Echo to prevent dependency on Echoes                | Low                            |                              |
| Multiple Language handling     | User can learn multiple languages and switch between them                                                       | Low                            |                              |

---

## **2. Beta Testing Scenarios**

### **2.1 User Roles**

[Define the different user roles that will be involved in testing, e.g., Admin, Regular User, Guest, External Partner.]

| **Role Name** | **Description**                                    |
| ------------- | -------------------------------------------------- |
| Admin         | Manage Echoes, Discussions, Lessons                |
| User          | Have access to the application to learn a language |

### **2.2 Test Scenarios**

For each core functionality, provide detailed test scenarios.

#### **Scenario 1: Login without SSO**

- **Role Involved:** User
- **Objective:** Ensure the user can sign in using an email and password.
- **Preconditions:** User has a registered account.
- **Test Steps:**

  1. User adds their email and password in the dedicated fields.
  2. User clicks on the "Sign in" button.

- **Expected Outcome:** User is connected and redirects to the Home view.

#### **Scenario 2: Create an account without SSO**

- **Role Involved:** User
- **Objective:** Ensure the user can create an account using an email and password.
- **Preconditions:** User does not have an account.
- **Test Steps:**

  1. User clicks the “Don’t have an account? Create one!” button.
  2. User adds their name, email and password in the dedicated fields.
  3. User clicks the “Sign up” button

- **Expected Outcome:** User is connected and redirects to the Home view.

#### **Scenario 3: Start a discussion with an Echo suggested**

- **Role Involved:** User
- **Objective:** Ensure the user can start a discussion with an Echo.
- **Preconditions:** User is logged in and on the Discussion Page.
- **Test Steps:**

  1. User chooses one of the places or topics suggested on the view.
  2. User navigates to a list of Echoes of this discussion.
  3. User chooses an Echo on this list and navigates to a chat with him.
  4. User is on the Chat Page with the chosen Echo.
  5. User sends a message to the Echo.

- **Expected Outcome:** The Echo responds to the user's message.

#### **Scenario 4: Start a discussion with an Echo**

- **Role Involved:** User
- **Objective:** Ensure the user can start a discussion with an Echo.
- **Preconditions:** User is logged in and on the Discussion Page.
- **Test Steps:**

  1. User wants to see all places or topics, so clicks on the “View all locations” or “View all topics” button
  2. User navigates to a list of discussions filter by places or topics
  3. User chooses a discussion on this list and navigates to a list of Echoes of this discussion.
  4. User chooses an Echo on this list and navigates to a chat with him.
  5. User is on the Chat Page with the chosen Echo.
  6. User sends a message to the Echo.

- **Expected Outcome:** The Echo responds to the user's message.

#### **Scenario 5: Start a discussion with an Echo from a search discussion**

- **Role Involved:** User
- **Objective:** Ensure the user can start a discussion with an Echo.
- **Preconditions:** User is logged in and on the Discussion Page.
- **Test Steps:**

  1. User searches with the search bar and/or add filters with the “Filters” button
  2. The discussions display all research discussions.
  3. User chooses a discussion on this list and navigates to a list of Echoes of this discussion.
  4. User chooses an Echo on this list and navigates to a chat with him.
  5. User is on the Chat Page with the chosen Echo.
  6. User sends a message to the Echo.

- **Expected Outcome:** The Echo responds to the user's message.

#### **Scenario 6: Resume a chat with an Echo**

- **Role Involved:** User
- **Objective:** Ensure the user can continue a chat with an Echo.
- **Preconditions:** User is logged in, on the Discussion Page and has already chatted with an Echo.
- **Test Steps:**

  1. User selects in the 3 recent chats the Echo they want to continue the conversation with.
  2. User navigates and is on the Chat Page with the chosen Echo.

- **Expected Outcome:** The user sees the previous messages and can continue the conversation.

#### **Scenario 7: See the errors on a message**

- **Role Involved:** User
- **Objective:** Ensure the user can see his errors on the chat page.
- **Preconditions:** User is logged in, on the Chat Page and has already send some messages.
- **Test Steps:**

  1. User sees the type of errors above the messages.
  2. User clicks on the message to see the errors.

- **Expected Outcome:** A modal opens with the details of the errors and an explanation of the error.

#### **Scenario 8: Discuss with the coach on an error**

- **Role Involved:** User
- **Objective:** Ensure the user can discuss about his errors on the modal page.
- **Preconditions:** User is logged in, on the Chat Page and has already send some messages.
- **Test Steps:**

  1. User clicks on the message to see the errors.
  2. User writes a message to the coach in the modal.
  3. User clicks on the “Send” button.

- **Expected Outcome:** The coach responds to the user's message in the modal.

#### **Scenario 9: Change their name and email**

- **Role Involved:** User
- **Objective:** Ensure the user can change their name and email.
- **Preconditions:** User is logged in, on the Profile Page.
- **Test Steps:**

  1. User clicks on the “Edit” button.
  2. User changes their name and email in the dedicated fields.
  3. User clicks on the “Save” button.

- **Expected Outcome:** The user has successfully changed their name and email.

#### **Scenario 10: Change the application language**

- **Role Involved:** User
- **Objective:** Ensure the user can change the application language.
- **Preconditions:** User is logged in, on the Profile Page.
- **Test Steps:**

  1. User clicks on the dropdown menu to choose the language.
  2. User selects the language they want to change.

- **Expected Outcome:** The application language is changed.

#### **Scenario 11: Disconnect**

- **Role Involved:** User
- **Objective:** Ensure the user can disconnect from the application.
- **Preconditions:** User is logged in, on the Home Page.
- **Test Steps:**

  1. User clicks on the “Disconnect” button in the Top Bar.

- **Expected Outcome:** The user is disconnected and redirected to the Sign In Page.

#### **Scenario 12: Delete his account**

- **Role Involved:** User
- **Objective:** Ensure the user can delete their account.
- **Preconditions:** User is logged in, on the Profile Page.
- **Test Steps:**

  1. User clicks on the “Delete my account” button.
  2. User confirms the deletion of their account.

- **Expected Outcome:** The user is disconnected and redirected to the Sign In Page and can't connect with this account anymore.

#### **Scenario 13: See the lessons**

- **Role Involved:** User
- **Objective:** Ensure the user can see the lessons.
- **Preconditions:** User is logged in, on the Lessons Page.
- **Test Steps:**

  1. User clicks on the “Lessons” button in the Navigation Bar.
  2. User selects a lesson to view.

- **Expected Outcome:** The user can see the lesson and its content.

#### **Scenario 14: Change the language to learn**

- **Role Involved:** User
- **Objective:** Ensure the user can change the language to learn.
- **Preconditions:** User is logged in.

- **Test Steps:**

  1. User clicks on the flag button in the Top Bar.
  2. User selects the language they want to learn.

- **Expected Outcome:** The user can see the lessons in the new language and the Echoes speak in this language.

---

## **3. Success Criteria**

| **Criterion** | **Description**                                                  | **Threshold for Success**                         |
| ------------- | ---------------------------------------------------------------- | ------------------------------------------------- |
| Stability     | No major crashes or critical bugs                                | No crash reported                                 |
| Usability     | Users can navigate and understand features with minimal guidance | 80% positive feedback from testers                |
| Performance   | Echo answer quickly                                              | Response within 5 seconds wiht 20 users connected |
| Relevance     | Echo talk about his topic                                        | Coherent conversation                             |
| Relevance     | The errors on the message                                        | See, report and explain correctly the errors      |
| Language      | Application is translate in multiples languages                  | At least 2 languages                              |

---

## **4. Known Issues & Limitations**

| **Issue**         | **Description**                                                    | **Impact** | **Planned Fix? (Yes/No)** |
| ----------------- | ------------------------------------------------------------------ | ---------- | ------------------------- |
| Meesages too long | The messages of the Echoes are too long                            | Medium     | Yes                       |
| Search Echo       | The search bar does not search for Echoes but only for discussions | Low        | No                        |

---

## **5. Conclusion**

This Beta Test Plan ensures that **Savy** is tested in a structured and efficient manner. By validating the core functionalities, refining the user experience, and ensuring feature stability, we aim to optimize Echoes for more relevant messages. The insights from this beta phase will help us address key issues and prepare for the final version of the project.
