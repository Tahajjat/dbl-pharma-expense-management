
# DBL Pharma Expense Management

An Android App designed for pharmaceutical sales representatives to streamline the process of managing expense claims, approvals, and reporting. The app offers a user-friendly interface for tracking expenses, submitting claims, and viewing approval statuses, making it an essential tool for pharma field teams.





## Features

- **Expense Claims:** Easily log and manage daily expenses with category and description options.
- **Approval Workflow:** Submit claims for approval and view approval status in real-time.
- **Reporting:** Generate and view summaries of expenses for custom time periods.
- **Data Storage:** Offline data storage with SQLite database for efficient and secure local storage.
- **API Integration:** Syncs with a central server to store data securely on a remote database.





# Getting Started

## Prerequisites
- Android Studio (latest version)
- An Android device or emulator running API level 21 (Lollipop) or higher

## Installation

**1. Clone the Repository:**

```bash
  git clone https://github.com/Tahajjat/dbl-pharma-expense-manager.git
```
**2. Open in Android Studio:**
- Open Android Studio and select Open an existing project.
- Navigate to the cloned repository and open it.

**3. Build and Run:**
- Sync your Gradle files.
- Connect your Android device or start an emulator.
- Run the app.

## Usage
1. **Log Expenses:** Open the app and tap on "Add Expense" to record a new expense. Enter the required details such as amount, category, and description.
2. **Submit for Approval:** After logging expenses, go to the "Submit Claims" section and select expenses to submit for approval.
3. **Check Approval Status:** View the approval status of each submitted claim in the "Approval Status" section.
4. **Generate Reports:** Use the "Reports" feature to view expense summaries over a selected period.




## Technologies
- **Frontend:** Java, XML
- **Backend:** SQLite (for local storage), API integration for remote data syncing
- **Tools:** Android Studio, Retrofit (for API calls)



## API Endpoints
The app integrates with an API to store data on a remote server. Here’s a summary of the main endpoints:

#### Get all expense list

```http
  GET /api/expenseList
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `api_key` | `string` | **Required**. Your API key |

#### Get employee expense list

```http
  GET /api/expenseList/${employee_id}
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `employee_id`      | `string` | **Required**. Employee_id of expense to fetch |




## License

This project is licensed under the MIT License. See the [LICENSE](https://choosealicense.com/licenses/mit/) file for more information.

## Contact
For questions or feedback, please reach out to tahajjat.tuhin@gmail.com.
