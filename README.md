# Chalkboard

Chalkboard is a tool which uses Google Cast. It allows a retail store to enter their product information in the Sender application HTML page, and then use Chromecast to cast the Receiver application HTML page to their Google Cast device. Useful for a business whose menu requires frequent changes.

## How It Works

Google Cast works using two parts. One part is a "Receiver" HTML5/JS application that runs and displays on the Cast device, and the other part is a Sender application which receives user input and sends relevant information to the Receiver. It is possible to create a "native" (installed via Google Play or the App Store) Sender application. This particular Sender application is also an HTML5/JS application, and as long as the user accesses the application using the Chrome browser, this Sender application should work regardless of OS.

## Prerequisites For Deployment

You will need:  
* A web server ready to host HTML and JavaScript
* A Google account with which to register a new Chromecast application

## Deployment

1. The repository files need to be placed into a public folder of a web server, with receiver.html and sender.html accessible from the web.
2. The [Google Cast publisher's dashboard](https://cast.google.com/publish/) needs to be visited. The location of receiver.html and sender.html need to be registered in the "Add New Application" section, and you should add your testing device to Cast Receiver Devices with "Add New Device" (without this, a Custom Receiver application may not be accessible via your Chromecast device until your application is fully published with Google) 
3. Execution of the application requires visiting sender.html in a Chrome browser. That's it!

## Authors

* **Google Cast Team** - *Initial work* - [Original Project](https://github.com/googlecast/CastHelloText-chrome)
* **Austin R. Scott** - [xeirxes](https://github.com/xeirxes)

See also the list of [contributors](https://github.com/xeirxes/chalkboard/contributors) who participated in this project.

## License

This project is licensed under the Apache License Version 2.0 - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* I'd like to thank Tim Buckley, proprietor of [Buckley's Pubs](https://www.buckleyspubs.com). Tim fosters a tight-knit, loyal team of employees who actively seek to improve our workplace, and this particular project was inspired by my own desire to improve Tim's establishment.