# api-assignment-tests

The repository is to collect and organize the postman collections used in the backend API Automation testing of enable assignment .

### How do I get set up?

1. Install Postman

   https://www.postman.com/downloads/

2. Install newman globally in your machine (Installation guide: https://www.npmjs.com/package/newman):

   ```
   npm install -g newman
   ```

   Install htmlextra reporter globally in your machine:

   ```
   npm install -g newman-reporter-htmlextra

   ```

   Run the enable api test collection using newman using below command:

   ```
   newman run -e "QA Environment.postman_environment.json" "Enable Collection.postman_collection.json" -r htmlextra

   ```

Note:

- Clone the repository and import the json collections in Postman to run the API requests locally.
- For QA environment json file, contact the repository owner.
- The above newman command can also be used to run the backend api test in CI/CD pipeline.
