# Lab Report 2
The topic for this lab report will cover servers and bugs. I teach you how to complete each step as well as tell you about my experience at each step. To help you better understand the steps I will include screenshots as well.
_____
## Part 1: Creating Your Web Server
To create your own basic server, first you must fork [this](https://github.com/ucsd-cse15l-f22/wavelet) repository and open it in VS Code. Then open the NumberServer.java file and make the changes in the handler class as shown below. 
'''
class Handler implements URLHandler {
    // The one bit of state on the server: a number that will be manipulated by
    // various requests.
    int num = 0;
    String s = "";

    public String handleRequest(URI url) {
        if (url.getPath().equals("/")) {
            return s;
        } 
         else {
            System.out.println("Path: " + url.getPath());
            if (url.getPath().contains("add-message")) {
                String[] parameters = url.getQuery().split("=");
                if (parameters[0].equals("s")) {
                    s += parameters[1]+'\n';
                    return s;
                }
            }
            return "404 Not Found!";
        }
    }
}
'''
