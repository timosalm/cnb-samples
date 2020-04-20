# Sample code for static files using the nginx CNB

## Running the sample locally
1. Clone the repository and move to the project folder
    ```
    git clone https://github.com/tsalm-pivotal/cnb-samples.git
    cd cnb-samples/static-files
    ```
2. Build the docker image
    ```
    pack build --builder cloudfoundry/cnb:cflinuxfs3 cnb-nginx-sample 
    ```
3. Run the docker image
    ```
    docker run --rm -p 80:8080 -e PORT=8080 cnb-nginx-sample 
    ```
4. Open the website in a browser
    ```
    open http://localhost:80
    ```
