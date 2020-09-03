
# linux-notes
A Linux (and Windows) application to replicate the Notes app from macOS. This is done by using Apple's iCloud service and Electron.


Note: This software is not affiliated with Apple

## Downloads
Linux
- [.deb](http://www.mediafire.com/file/2o1qiumu1lq2bqs/notes-linux_1.0.0_amd64.deb/file)

## Usage
On Linux, by default the application will install to your `/usr/share/applications` folder.
On Windows, you can find it on your `C:/User/Desktop` folder.

After opening the app, sign in with your Apple ID. You may be prompted for two factor authentication. Upon success, the app will open the notes application with your iCloud data.

## Screenshots


## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

First, install a recent version of [Node.js](https://nodejs.org/en/download/). I reccomend downloading the `Current` or `LTS` version. Once downloaded, run through the installer and confirm everything works by typing the following command in Terminal.
```
# This command should print the version of Node.js
node -v
# this command should print the version of npm
npm -v
```

You will also require a code editor such as Microsoft's [Visual Studio Code](https://code.visualstudio.com/download).

### Installing

To get the development environment running, clone the repository to your computer using git.

```
git clone https://github.com/tariqsyed1/notes-linux.git
```

Change into the notes-linux directory in Terminal and open the notes-linux directory in your code editor.

```
cd notes-linux
```
Start the application with Electron using npm

```
npm start
```

You should be prompted with the app running in the [Chromium](https://en.wikipedia.org/wiki/Chromium_(web_browser)) framework. 
After making changes to the program in your editor, run `rs` in the active terminal running the app to restart the application and see the changes take effect.

Note: I'd reccomend looking at the [Electron Architecture](https://www.electronjs.org/docs/tutorial/application-architecture) to understand how the code works.

## Deployment

To deploy your build on a live system, simply type the following in your terminal.
```
# Change to directory
cd notes-linux
# Use npm to create distributable 
npm run make
# ...output...
```
`npm run make` will create a distributable for the system you're running it on. The file can be found in the /out directory created after the command completes.

## Built With

* [Electron](https://www.electronjs.org/) - The web framework used
* [Nodejs](https://nodejs.org) - Runtime environment
* [iCloud](https://apple,ca/icloud) - For the notes data

## Authors

* [Tariq Syed](https://github.com/tariqsyed1)


## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details

Enjoy! :+1:
