### **BETA TEST PLAN – Savy**

## **1. Core Functionalities for Beta Version**

| **Feature Name**               | **Description**                                                                                                 | **Priority (High/Medium/Low)** | **Changes Since Tech3**      |
| ------------------------------ | --------------------------------------------------------------------------------------------------------------- | ------------------------------ | ---------------------------- |
| Send messages                  | User sends a message to an Echo with a dedicated interface                                                      | High                           |                              |
| Receive messages               | User receives a response to the message they sent                                                               | High                           |                              |
| Messages history               | User can see the message history in a conversation                                                              | High                           |                              |
| Create Echoes                  | User has access to a large panel of Echoes                                                                      | High                           |                              |
| Chat Page                      | User uses this page to chat with an Echo                                                                        | High                           |                              |
| Discussion List Page           | The list of all available discussions where the user can choose                                                 | High                           |                              |
| Discussion Page                | The main page of the discussion where the user can see their recent chats, 3 random topics, and 3 random places | High                           |                              |
| Sign In / Sign Up Page w/o SSO | User can sign in or create an account with their email and password                                             | High                           | Split the w/ SSO and w/o SSO |
| Implement Text To Speech       | User can listen to the Echo speaking to them                                                                    | Medium                         |                              |
| Send voice messages            | User sends a voice message to an Echo                                                                           | Medium                         |                              |
| Navigation Bar                 | User can navigate through Home/Discussion/Stats/Lessons                                                         | Medium                         |                              |
| Top Bar                        | User can switch languages and view their profile                                                                | Medium                         |                              |
| See Errors on Messages         | User can see errors on messages when they send one                                                              | Medium                         | Added more precisions        |
| Profile Page                   | User can view and edit their profile information                                                                | Medium                         |                              |
| Implement Mouth Movement       | The mouth of the Echo moves when it speaks                                                                      | Low                            |                              |
| Sign In / Sign Up Page w/ SSO  | User can sign in or create an account with Google/Apple SSO                                                     | Low                            | Split the w/ SSO and w/o SSO |
| Home Page                      | The page regroups a summary of Discussion/Stats/Lessons                                                         | Low                            |                              |
| Lessons Page                   | User can access and view lessons on the language they are learning                                              | Low                            |                              |
| Stats Page                     | User can view their statistics and progress                                                                     | Low                            | Added in dedicated Page      |
| Moderation Savy                | The AI Savy moderates the messages between the user and the Echo to prevent dependency on Echoes                | Low                            |                              |
| Alphabet Learning              | User can learn the alphabet                                                                                     | Low                            |                              |
| Link courses with Echoes       | The courses can redirect to chat with an Echo to discuss what they have learned                                 | Low                            |                              |
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

---

## **3. Success Criteria**

| **Criterion** | **Description**                                                  | **Threshold for Success**          |
| ------------- | ---------------------------------------------------------------- | ---------------------------------- |
| Stability     | No major crashes or critical bugs                                | No crash reported                  |
| Usability     | Users can navigate and understand features with minimal guidance | 80% positive feedback from testers |
| Performance   | Echo answer quickly                                              | Response within 5 seconds          |
| Relevance     | Echo talk about his topic                                        | Coherent conversation              |
| Language      | Application is translate in multiples languages                  | At least 2 languages               |

---

## **4. Known Issues & Limitations**

| **Issue**         | **Description**                                                    | **Impact** | **Planned Fix? (Yes/No)** |
| ----------------- | ------------------------------------------------------------------ | ---------- | ------------------------- |
| Search Echo       | The search bar does not search for Echoes but only for discussions | Medium     | Yes                       |
| Meesages too long | The messages of the Echoes are too long                            | Medium     | Yes                       |

---

## **5. Conclusion**

This Beta Test Plan ensures that **Savy** is tested in a structured and efficient manner. By validating the core functionalities, refining the user experience, and ensuring feature stability, we aim to optimize Echoes for more relevant messages. The insights from this beta phase will help us address key issues and prepare for the final version of the project.
