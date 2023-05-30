# Google_Secret_Manager
How to use Google Secret Manager in Firebase Cloud Function




1.Go to the Google Cloud Console: https://console.cloud.google.com/
2. Open your project.
3. Navigate to the "IAM & Admin" -> "IAM" page.
4. Look for the service account used by your Cloud Function. It should be in the format <project-id>@appspot.gserviceaccount.com.
5. Click on the service account to open the IAM policy editor.
6.Click the "ADD" button to add a new permission.
7. In the "Select a role" dropdown, search for "Secret Manager Secret Accessor" and select the appropriate role, such as "Secret Manager Secret Accessor".
8. In the "Filter" field, enter the name of your secret, for example, projects/260204983617/secrets/clientId.
9. Select the secret from the dropdown.
10. Click the "SAVE" button to grant the permission.
By granting the "Secret Manager Secret Accessor" role or a similar role to the service account, you are allowing it to access the latest version of the secret.
