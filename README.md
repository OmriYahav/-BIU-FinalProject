# RED PROJECT

## Team Members:
- Omri Yahav: omriyx@gmail.com 
- Itzik Bibi: bibi.itzhak@gmail.com
- Eliraz Oved: ovedeliraz96@gmail.com

## Institute:
Bar Ilan University 🎓

## Project Description
Please provide a detailed description of your project.

## Installation

1. Make sure you have Docker installed on your system.

2. Clone this repository to your local machine using the following command:

   ```bash
   git clone https://github.com/OmriYahav/-BIU-FinalProject
   ```

3. Change to the project directory:

   ```bash
   cd -BIU-FinalProject
   ```

4. Build the Docker image:

   ```bash
   docker build -t pingpong-app .
   ```

5. Run the Docker container:

   ```bash
   docker run -d -p 5005:5005 pingpong-app
   ```

## Usage

1. The application is now running inside a Docker container on `http://localhost:5005/`.

2. Send a GET request to `http://localhost:5005/ping` with a JSON body containing a 'content' key and the value 'ping'. For example:

   ```bash
   curl -X GET -H "Content-Type: application/json" -d '{"content": "ping"}' http://localhost:5005/ping
   ```

3. The application will respond with a JSON containing a 'message' key and the value 'pong'.

   ```
   {"message": "pong"}
   ```


