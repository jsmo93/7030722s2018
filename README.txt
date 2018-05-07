Code Disclosure:
  Android Application:
    My Work:
      All of the code in the provided folder is my original work, except for the Libraries listed below. This includes all layout files, adapters, fragments and activities.
    Libraries:
      RxJava2 (Unmodified) – Used to chain and simplify Retrofit calls
      RXAndroid2 (Unmodified) – Used to chain and simplify Retrofit calls
      GSON (Unmodified) – Used to serialize JSON
      Retrofit (Unmodified) – Used to make network calls
      Retrofit GSON Converter (Unmodified) – Used to serialize JSON
      Retrofit RxJava2 Adapter (Unmodified) – Used to chain and simplify Retrofit calls

    Icons:
      Google Material Design Icons (Unmodified)

    Client Images:
      Credit.png – Free stock photo from Pexels.com (Scaled/Cropped)
      Power.png - Free stock photo from Pexels.com (Scaled/Cropped)
      Pizza.png - Free stock photo from Pexels.com (Scaled/Cropped)

  Rails Application:
    My Work:
      All of the code in the provided folder is my original work, except for the Library listed below. This includes all models, controllers, migrations, and seeds.

    Libraries:
      Valid_Email2 (Unmodified) – https://github.com/lisinge/valid_email2 - Use to check for valid emails

    Design Resources:
      Open Web Applications Security Project (OWASP) – Secure Coding Guidelines: Quick Reference Guide which can be found here: https://www.owasp.org/index.php/OWASP_Secure_Coding_Practices_Checklist. I used this guide to understand and implement best practices in my server design

Building, Installing and Running:
  Installing the Android Application from Android Studio:
    1) Download and install Android Studio using these instructions: https://developer.android.com/studio/install
    2) Select "Open an Existing Android Studio project" and point to the IdentityGuardApp folder.
    3) Android Studio will begin loading the application. If you see a message which says that you are missing a version of the SDK or Build Tools, click the install link provided in the error. Ignore any requests to upgrade the projects Gradle version.
    4) Turn on an Android device running Android 6.0 (Marshmallow) or later. Enable USB Debugging as described here: https://developer.android.com/studio/debug/dev-options
    5) Plug in the device and press the run (or play) button to launch the app. You may be asked if you trust the computer to be used as a debugger, press the yes button
    6) Make sure that the device is connected to the same network as the server
    Note: The app may look distorted on smaller or lower resolution screens.

  Installing the Rails Application using RubyMine:
    1) Follow this tutorial to install the Ruby Version Monitor (RVM), stop at the section labeled "Rails", do not do "gem install rails --version 5.0.0": http://blog.teamtreehouse.com/installing-rails-5-linux
    2) In the terminal now setup for login shell, navigate into the IdentityGuardApi folder
    3) Type 'gem install bundler' to install the bundler
    4) When the installation finishes, type 'bundle install --path ./local_gems', this will create a local gems folder and install the gems needed to use the server
    5) When the installation finishes, type 'rake db:drop db:create db:migrate db:seed', this will create a new database and seed it with the client information built into the android app
    6) When the database setup is finished, type 'rails s', this will start the server in development mode
    7) In another terminal window, type 'ifconfig' and record the IP Address of the machine. The app must be pointed to the server using this address