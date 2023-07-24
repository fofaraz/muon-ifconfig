#ifconfig

This project is a simple Express application built with Node.js that allows you to retrieve your IP address when calling the `/` route.

##Prerequisites
Before running the ifconfig project, ensure you have the following installed on your system:

- Node.js (https://nodejs.org)
- npm (Node Package Manager, comes with Node.js)

##Installation

1. Clone this repository to your local machine or download the source code as a zip file and extract it.
2. Open a terminal or command prompt and navigate to the project directory.
3. Install the required dependencies by running the following command:
`npm install`

##Usage
1. To start the ifconfig server, copy `.envexample` file and rename it to `.env` then use the following command:
`npm start`
2. The server will be running at `http://localhost:3002` by default.

3. Open your web browser or use tools like curl or Postman to make an HTTP GET request to the / route.

4. The server will reply with a JSON object containing your IP address:

    ```
    {
      "success": true,
      "ip_addr": "YOUR_IP_ADDRESS"
    }
    ```
##Example
Using curl, you can make a request to the `/` route and retrieve your IP address:

`curl http://localhost:3000`

Sample response:
```
{
  "success": true,
  "ip_addr": "192.168.1.100"
}

```
