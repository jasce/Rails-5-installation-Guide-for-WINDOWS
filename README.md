# Rails-5-installation-Guide-for-WINDOWS

### Installing Rails 5 on WINDOWS can be a pain. So, here I'm presenting the simple installation guide for the awesome web framework.

#### First, we need an installation of the Ruby programming language. We’re going to use a precompiled version of Ruby called Ruby Installer.


 1. Download and run [Ruby Installer version 2.3.1](https://bintray.com/oneclick/rubyinstaller/rubyinstaller/2.3.1) or [Ruby Installer version 2.2.5](https://bintray.com/oneclick/rubyinstaller/rubyinstaller/2.2.5)from rubyinstaller.org. (For convenience, I have linked directly to the bintray). Note: Make sure to download RubyInstaller version > 2.2.2.
 

 2. Run downloaded .exe file.An installation wizard will open. Check “Add Ruby executables to your PATH”, then click Install. Wait while the installer runs, and click Finish when done
 

 3. To access Ruby, go to the Windows menu, click All Programs, scroll down to Ruby, and click “Start Command Prompt with Ruby”. A command prompt terminal will open. If you type `ruby -v` and press Enter, you should see the Ruby version number that you installed.
 

 4. Download the [Ruby Development Kit](http://dl.bintray.com/oneclick/rubyinstaller/DevKit-mingw64-32-4.7.2-20130224-1151-sfx.exe). (This download also originates from rubyinstaller.org, and is also hosted on bintray.com.)
 

 5. When it’s done, go to your downloads folder and double-click the DevKit executable.We need to specify a folder where we’re going to permanently install the DevKit. I recommend installing it in the root of your hard drive, at `“C:\RubyDevKit“`. (Don’t use spaces in the directory name.)
 

 6. Back in your command prompt, change to the the DevKit directory. (“Directory” is another name for a folder.) Type `“cd C:\RubyDevKit“`, or whatever other directory name you installed it in.
 

 7. Next we need to run a Ruby script to initialize the DevKit setup. Type `ruby dk.rb init`. Now we’ll tell that same script to add the DevKit to our Ruby installation. Type `ruby dk.rb install`.
 

 8. Download the latest Certificate, [GlobalSignRootCA.pem](https://raw.githubusercontent.com/rubygems/rubygems/master/lib/rubygems/ssl_certs/index.rubygems.org/GlobalSignRootCA.pem). ####IMPORTANT:### File must have .pem as extension. Browsers like Chrome will try to save it as plain text file. Ensure you change the filename to end with .pem after you have downloaded it.
 

 9. Now Loacte ssl_certs directory. Usually its given at `C:\Ruby22\lib\ruby\2.2.0\rubygems\ssl_certs`. Place the downloaded certificate into this directory.
 
 
10. Now we are all set to download rails as a ruby gem. In your command prompt, type:

`gem install rails --version 5.0.0`.

This will ensure you’re downloading the correct version of the gem. Once you press Enter, the “gem” program will download and install that version of the Rails gem, along with all the other gems Rails depends on.

### 11. One last thing. . . Some libraries that Rails depends on require a JavaScript runtime to be installed. Please install Node.js so that those libraries work properly.


# I hope this works !!
