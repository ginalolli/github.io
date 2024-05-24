**Getting Started with Docker**

Its simple to start using Docker for your local development environment, just follow these steps:

1. **Ensure Docker is Running**
  Check that you have the Docker application up and running on your computer.

2. **Navigate to Devilbox Directory**
   Launch the terminal and navigate to the Devilbox directory using the command:
   ```
   cd ~/Development/devilbox
   ```

3. **Start the Environment**
   Start the entire environment by running the following command:
   ```
   docker-compose up -d php php81 httpd mysql
   ```

4. **Stopping the Environment**
   In order to stop all Docker services, use the command:
   ```
   docker-compose stop
   ```

**Getting to Work**

Make sure you have two terminal tabs open for easy development:

1. **Mac Terminal (mac-shell):**
   Go to your project directory using:
   ```
   cd ~/Development/www/your_project_directory
   ```
   If navigating here for the first time, run `composer install` or `composer update` to set up dependencies.

2. **Devilbox Shell (devilbox-shell):**
   a. Navigate to the Devilbox directory:
      ```
      cd ~/Development/devilbox
      ```
   b. Run Devilbox shell script:
      ```
      ./shell81.sh
      ```
   c. Enter your project directory:
      ```
      cd evbox.com
      ```
      (Run `composer install` or `composer update` if needed.)

   d. Start watching for changes:
      ```
      npm run watch
      ```

**Mac-Shell Commands:**
- Use Git
- Open the project in Visual Studio Code:
  ```
  cd ~/Development/www/evbox.com
  code .
  ```
- Install Node.js modules:
  ```
  npm install
  ```

**Devilbox-Shell Commands:**
- Run Node.js:
- Run Gulp tasks:
  ```
  gulp compile
  gulp watch
  ```
- Manage Composer:
  ```
  composer update
  ```

**Stylelint Commands:**
In case of pipeline failures, use:
```
npm run eslint
npm run stylelint
npm run stylefix // Auto-fix style issues
```

**SSH Key Password for Bitbucket:**
If prompted for an SSH key password:
1. Run in any terminal window:
   ```
   eval "$(ssh-agent -s)"
   ssh-add
   ```
2. Enter the password. Retrieve it from Keychain Access by searching for `id_ed`.
   Right-click on the relevant entry and copy the password.

**Devilbox Dashboard:**
Access the Devilbox dashboard at [http://localhost/index.php](http://localhost/index.php).

**Tip:**
To copy your SSH key, run:
```
cat ~/.ssh/id_rsa.pub
```

With these steps, you should be ready to start using Docker for your local environment.


