# Frontend Coding Challenge: Enhanced Onboarding Page
A little task to show us some of your UI/UX SuperPowers

## Overview
For TaxP@rrot, the user onboarding experience is paramount, especially in accurately capturing tax-related information. This challenge focuses on developing an Onboarding Page that caters to diverse user types, collecting base information, and then guiding users through specifying their income and expenses types.

## User Types
There are three primary user types for this application:
1. **Salaried Employee**: Individuals who earn a regular income from employment, including those with additional side business income.
2. **Business Owner**: Entrepreneurs who own and operate a business, needing to manage both personal and business-related taxes.
3. **PAYE Filer**: Business owners or payroll managers responsible for filing Pay-As-You-Earn (PAYE) taxes for employees.

## Onboarding Flow Process

1. **Select User Type**: Users start by selecting their user type (Salaried Employee, Business Owner, PAYE Filer). This choice determines the subsequent information collected during the onboarding process.

2. **Base Information Collection**:
To ensure our onboarding process is comprehensive, we require the collection of specific information for each user type. Below is a predefined list of the information you should include in your application:
   - **All Users**: Collect common information applicable to all users. You might want to collect information like:
     ```
     Name: Full name of the user
     Email Address: User's email address for contact purposes
     Contact Number: User's phone number
     ```
   - **Salaried Employees**: Request personal tax ID and any relevant information about their employment. Typical information collected here include:
     ```
     Personal Tax ID: The tax identification number for the individual
     Employer's Name: Name of the company where the user is employed
     Employment Start Date: When the user began their current employment
     ```
   - **Business Owners**: Ask for business name, business tax ID, and the nature of the business. Information like the below could be relevant:
     ```
     Business Name: The official name of the business
     Business Tax ID: Tax identification number for the business
     Type of Business: The sector or nature of the business (e.g., Retail, Services, Manufacturing)
     ```
   - **PAYE Filers**: Require details on the number of employees and business information for PAYE purposes. Information like the below could be relevant here:
     ```
     Number of Employees: How many employees the business has
     Payroll Contact: The contact information for the person managing payroll
     PAYE Registration Number: The registration number for PAYE with the tax authority
     ```

Ensure your application includes form fields to capture all the above information accurately. Maybe you could use conditional logic to display relevant fields based on the user's selected type.

3. **Income and Expenses Section**:
   After collecting base information, guide users to specify their income sources and expenses. The availability and type of options in this section might vary based on the user type selected at the beginning. You can use the predefined list of income and expneses below and be creative in how you present this to the user:

```
const incomes = [
  'Rent', 'Sales of Shares', 'Performing a Service', 'Cryptocurrency', 
  'Sales of an Asset', 'Freelance Job', 'Selling my Car', 'Income Interests', 
  'Other Sources not Mentioned', 'Income from Abroad'
];

const expenses = [
  'Medical Bills', 'Office Expenses', 'Charitable Donations', 'Health Savings', 
  'School Loans', 'Educational Fees', 'Child Care Costs', 'Expenses Related to my Job', 
  'Other Business Expenses', 'Capital Expenses in Machines', 'Farm Tools'
];
```

## Deliverables

- **Source Code**: Push your complete source code to a public GitHub repository.
- **README.md**: Include setup instructions, how to run your project, and any assumptions or important decisions you made.

## Evaluation Criteria

- **Adherence to Requirements**: How well does the solution follow the specified user types and onboarding flow?
- **Code Quality and Structure**: Is the code clean, well-organized, and maintainable?
- **User Experience**: Is the onboarding process intuitive, and does the UI facilitate a smooth flow from start to finish?
- **Problem Solving and Creativity**: How effectively are dynamic form adjustments and user type variations handled?

## Specific Requirements

### Build Setup
This coding challenge is not designed to evaluate how you set up your build, but rather to give you a chance to build something small to demonstrate how you approach problem-solving, design and user experience. We recommend that you use `create-react-app` which is simple to get started with react.
 - Use React
 - Provide a README file and add information on how to build and/or run the project locally. This file can also include your thought process and any explanation.
 - Push the application to a public github repo and provide us with a link.
 - If you want to, feel free to use any boilerplate projects that bootstap the project for you, (but we recommend create-react-app, as noted above).
 - Add some styles, make it pretty.
 - There are lots of autocomplete projects out there, we're not interested in those. We want to see you.
 - Feel free to go above and beyond

### Dynamic Form Logic
- Implement logic to dynamically adjust the form based on the selected user type.
- Ensure the transition between sections is smooth, with clear instructions for the user on what is expected.

### Income and Expense Selection for Business Owners and Salaried Employees
- For **Business Owners** and **Salaried Employees**, provide a list of possible income sources and expenses to select from. Use the provided datasets but consider the relevance based on the user type.
- Implement a mechanism (e.g., checkboxes, toggle switches (feel free to be creative here)) that allows for multiple selections and the ability for users to add items not listed.

### Information Validation and Submission
- Validate user inputs before submission to ensure all required fields are filled and correctly formatted.
- On submission, simulate a backend post request (you can mock this using tools like MirageJS or json-server if you like) and provide feedback to the user upon success or failure.

### UI/UX Design
- The interface should be intuitive, with clear indications of mandatory versus optional fields.
- Use tooltips or modal dialogs to offer additional information for certain fields or selections without cluttering the main UI.


## Submission

Submit your GitHub repository link through tech@taxparrot.com by Tuesday February 13th 2024. For any questions or clarifications, please contact tech@taxparrot.com.

