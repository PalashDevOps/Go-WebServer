# Go-WebServer

A simple, efficient web server implemented in Go (Golang). This project demonstrates the basics of building and running a web server using Go, showcasing how to serve static files effectively.

I have used two function in this web server project 
1 - hellohandler - to implement the logic to print custom values ex. helloworld!

2- formhandler -  to enroute the trafic to your static content

3- for default i.e. index.html I have used http.Handle function from the http package

##Packages used in this Project

1. fmt
2. net/http
3. log

## Features

- Serves static content (index.html and form.html).
- Lightweight and easy to extend.

---

## Prerequisites

Before running the project, ensure you have the following installed on your system:

- **Golang**: [Download and install Go](https://golang.org/dl/).
- **Git**: [Download and install Git](https://git-scm.com/).

Verify your installations:

```bash
$ go version
$ git --version
```

---

## Installation

Follow these steps to clone and run the project:

1. Clone the repository:

```bash
git clone https://github.com/PalashDevOps/Go-WebServer.git
```

2. Navigate to the project directory:

```bash
cd Go-WebServer
```

3. Build the project:

```bash
go build -o webserver
```

---

## Running the Server

After building the project, you can start the server using the following command:

```bash
./webserver
```

By default, the server listens on port **8080**. Open your browser and navigate to:

```
http://localhost:8080
```

The server will serve static files from the `static/` folder.

---

## Project Structure

Here is an overview of the project structure:

```
Go-WebServer/
├── main.go        # Entry point for the application
├── static/        # Static files (HTML, CSS, JS, etc.)
└── README.md      # Documentation
```

### Explanation of Key Files

- **main.go**: Initializes the server and serves static files from the `static/` directory.
- **static/**: A folder containing your HTML, CSS, and JavaScript files.

---

## Extending the Project

1. **Serving Additional Static Files**:
   - Add your files to the `static/` directory.

2. **Changing the Default Port**:
   - Modify the port number in `main.go`:

     ```go
     log.Fatal(http.ListenAndServe(":8080", nil))
     ```

---

## Contributions

Contributions are welcome! Feel free to open an issue or submit a pull request for improvements or new features.


---

## Contact

For questions or feedback, reach out to [PalashDevOps](https://github.com/PalashDevOps).

Happy coding!
