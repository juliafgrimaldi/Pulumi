# Pulumi

- Installing pulumi on Linux <br>
 --Running the installation script:
 ```sh
 $ curl -fsSl https://get.pulumi.com | sh
 ```
 After installing pulumi, it's required to install the language runtime, in this case, python.
 
  ```sh
 $ apt get update
 $ sudo apt install python3-venv 
 ```
 - Creating a new project
  ```sh
 $ pulumi new
 ```
 When creating a new project, you can choose a template from the list. For this project I used gcp-python.
 
 !note: It's possible to create a new project already with the template you want. For exemple:
   ```sh
 $ pulumi new gcp-python
 ```
 - After that, you'll proceed to configurate your newest project. Hit ENTER for default values.
  <br>Lastly you will need to enter your project id from gcp.
 
    ```sh
   $ gcp:project: The Google Cloud project to deploy into: [your project id]
   ```
  - Let's have a look at the generated project files:
    - The python file (main.py) is where you define your stack resources.
    - Pulumi.yaml defines the project
    - Pulumi.dev.yaml defines the configuration values for the stack we initialized
    
  
  
