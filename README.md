# Web_dev_project
Final proj, CS web dev

## CRUD Functionality:

The application displays a number retrieved from Firebase and provides buttons to manipulate this number:

* **Read:**
    * Upon loading, the webpage reads the current value of the counter from the Firebase Firestore database and displays it.
    * If no data exists, it will indicate that ("No data yet!").
* **Increment Number (+1) Button (Update):**
    * When clicked, this button increments the current counter value in Firebase by 1.
    * The webpage display updates in real-time to show the new value.
* **Reset Number (to 0) Button (Create/Update):**
    * When clicked, this button sets the counter's value to `0` in Firebase.
    * If the counter document doesn't exist in Firebase, this action will create it and set its value to `0`. If the document already exists, its `value` field is simply updated to `0`.
    * The webpage display updates to show `0`.
* **Delete Number Button (Delete):**
    * When clicked, this button completely deletes the counter document from the Firebase Firestore database.
    * The webpage display will then update to indicate that no data is available (e.g., "No data yet!").

---
## Key needed:

* To make this work with firebase asynchronously we need the firebase config snippet in our index file directly, which is what I did, without the API credentials it won't sync/work.