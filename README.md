# **2025-OBJPROG-LAB013**
Week 05 - Methods in Java

Laboratory # 13 - Guided Coding Exercise 2: Parameters vs. Arguments

## **Instructions**

### **Step 1.1: Accept the Assignment**

   1. Click on the assignment link provided by your instructor.
   2. GitHub Classroom will create a **private repository** under your GitHub account.
   3. After the repository is created, click **"Go to Repository"** to view your assignment.

---

### **Step 1.2: Setup your Git Environment**
Only perform this if this is the first time you will setup your Git Environment

   1. Create a GitHub Account:
   ```bash
   https://github.com/signup?source=login
   ```
      
   2. Download and Install Git on your Laptop/Desktop:
   ```bash
   https://git-scm.com/downloads
   ```
   
   3. Create a Folder in your Laptop/Desktop
   4. Right-click anywhere in the created folder and select "Open Git Bash Here".
   5. In the Git Bash Terminal, set your git name, perform command:
   ```bash
   git config --global user.name "Your Name"
   ```
   
   6. In the Git Bash Terminal, set your git email, perform command:
   ```bash
   git config --global user.email "your.email@example.com"
   ```
   
   7. Create your SSH Key, just follow the instructions, no need to provide filename and passphrase. In the Git Bash Terminal, perform command:
   ```bash
   ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
   ```
   
   8. Copy your SSH Keys into clipboard. In the Git Bash Terminal, perform command:
   ```bash
   clip < ~/.ssh/id_rsa.pub
   ```
   
   9. Log in to your GitHub account.
   10. In the upper-right corner of GitHub, click your profile picture and select Settings.
   11. In the left sidebar, click on SSH and GPG keys.
   12. Click the New SSH key button.
   13. In the Title field, give the key a recognizable name (e.g., "My Windows Laptop").
   14. In the Key field, CTRL + V or paste the keys copied into your clipboard. Save the key.
   15. Go Back to terminal, use command:
   ```bash
   ssh -T git@github.com
   ```

### **Step 2: Clone the Repository to Your Local Machine**

   1. On your repository page, click the green **"Code"** button.
   2. Copy the repository URL (choose HTTPS for simplicity).
   3. Open your terminal (or Git Bash, Command Prompt, or PowerShell) and run:
   
   ```bash
   git clone <git_repo_url>
   ```
   
   4. Navigate into the cloned folder:
   
   ```bash
   cd <git_cloned_folder>
   ```

### **Step 3: Complete the Assignment**

**Laboratory # 13 - Guided Coding Exercise 2: Parameters vs. Arguments**

   **Objective:**
   - Differentiate between parameters and arguments.
   - Understand that parameters are defined in method declarations, while arguments are the actual values passed during a method call.

   **File Naming Convention:**
   - `ParametersAndArguments.java`

   **Desired Output:**
   ```txt
   The calculated area is: 150
   ```

   **Notable Observations (to be discussed after completing the exercise):**
   - In the calculateArea method definition, width and height are the parameters.
   - When calling calculateArea in main, roomWidth and roomHeight are the arguments that are passed to the method.
   - The values of the arguments are used to replace the parameters when the method is executed.

   **Java Programming Best Practices:**
   - Use clear and descriptive names for both parameters and arguments to avoid confusion.
   - Choose names that indicate the purpose of the parameter or argument (e.g., roomWidth clearly suggests it holds the width of a room).
      
   **Step-by-Step Instructions:**

   1. Setup Class and Main Method
      - Create a file named `ParametersAndArguments.java`.
      - Define the class `ParametersAndArguments` and the `main` method.
      ```Java      
      public class ParametersAndArguments {
          public static void main(String[] args) {
      
          }
      }
      ```
            
   2. Create the calculateArea Method (Part 1)
      - After the closing curly brace of main, type public static int calculateArea(int width, int height) {}
      ```Java
      public class ParametersAndArguments {
          //... (main method)...
      
          public static int calculateArea(int width, int height) {
      
          }
      }
      ```

   3. Create the calculateArea Method (Part 2)
      - Inside calculateArea, add these lines:
         - int area = width * height;
         - return area;
      ```Java
      public class ParametersAndArguments {
          //... (main method)...
      
          public static int calculateArea(int width, int height) {
              int area = width * height;
              return area;
          }
      }
      ```

   4. Declare Variables in main
      - In the main method, add these lines:
         - int roomWidth = 10;
         - int roomHeight = 15;
      ```Java
      public class ParametersAndArguments {
          public static void main(String[] args) {
              int roomWidth = 10;
              int roomHeight = 15;
          }
          //... (calculateArea method)...
      }
      ```

   5. Call calculateArea
      - In main, add this line: int area = calculateArea(roomWidth, roomHeight);
      ```Java
      public class ParametersAndArguments {
          public static void main(String[] args) {
              //... (variable declarations)...
              int area = calculateArea(roomWidth, roomHeight);
          }
          //... (calculateArea method)...
      }
      ```

   6. Print the Result
      - In main, add this line: System.out.println("The calculated area is: " + area);
      ```Java
      public class ParametersAndArguments {
          public static void main(String[] args) {
              //... (other code in main)...
              System.out.println("The calculated area is: " + area);
          }
          //... (calculateArea method)...
      }
      ```

   7. Compile and Run
       - Save the file as `ParametersAndArguments.java`.
       - Compile the code using `javac ParametersAndArguments.java` in your terminal or command prompt.
       - Run the compiled code using `java ParametersAndArguments`.

   **Conclusion**
   This exercise clarified the distinction between parameters and arguments in Java methods. Parameters act as placeholders in the method definition, while arguments are the actual values supplied during the method call. Understanding this difference is crucial for writing and using methods effectively in your Java programs.

### **Step 4: Push Changes to GitHub**
Once you've completed your changes, follow these steps to upload your work to your GitHub repository.

1. Check the status of your changes:
   Open the terminal and run:
   
   ```bash
   git status
   ```
   This command shows any modified or new files.
   
2. Stage the changes:
   Add all modified files to staging:
   
   ```bash
   git add .
   ```
   
3. Commit your changes:
   Write a meaningful commit message:
   
   ```bash
   git commit -m "Submitting OBJPROG Week 05 - Laboratory # 13"
   ```
   
4. Push your changes to GitHub:
   Upload your changes to your remote repository:
   
   ```bash
   git push origin main
   ```
