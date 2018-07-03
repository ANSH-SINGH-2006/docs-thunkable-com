# Screen

 ![](../../../.gitbook/assets/screen-icon.png)

{% hint style="info" %}
On Thunkable, there is a recommendation of 10 screens per app. Please [read these instructions](https://thunkable.gitbook.io/thunkable-docs/thunkable-classic-android/2-create/app-limits) if you want to exceed 10 screens
{% endhint %}

Screens are where you set layouts, program the initial opening of the app and the navigation. Screen1 is also where you set many of your app level properties.

* [Align elements on a screen](screen.md#align-elements-on-a-screen)
* [Add a new screen](screen.md#add-a-new-screen)
* [Open a screen with a button](screen.md#open-a-screen-with-a-button)
* [Pro-tip: Branding splash screens](screen.md#-pro-tip-branding-splash-screens)
* [App settings \(Screen 1 only\)](screen.md#app-settings-screen1-only)
  * [Rename app and upload icon](https://docs.thunkable.com/android/create.html#3--rename-app-and-upload-app-icon)
  * [Edit about this application](https://docs.thunkable.com/android/create.html#about-this)
* [Appearance](screen.md#appearance)
* [Functionality](screen.md#functionality)

### Align elements on a screen

![](../../../.gitbook/assets/align-screen-fig-1.png)

### Add a new screen

![](https://lh6.googleusercontent.com/1oEzLB4YgohJ9xkkqyOox_Ljr9gbVxreM8EfuVqC0LX0jni6rhmNbBvZzbrqCCng0dHfeKh_g2bPthx2pfKrTpHZx3jOpAel5K_zXQPs3UyabZ1dYzq0VD4ikRJ0krCWMPZkpJZg)

### Open a screen with a button

![](../../../.gitbook/assets/open-screen-fig-1.png)

### ![](../../../.gitbook/assets/pro-tip-icon.png) Pro-tip: Branding splash screens

Apps often take a few seconds to load which can be very discouraging to a new user. One way to create space for this loading period is by adding a screen with your logo and letting it run for a given amount of time \(we have found 3 seconds to feel just about right in most cases\).

You can [watch this tutorial](https://www.youtube.com/watch?v=9u365ejwTqg) to learn more

### App settings \(Screen1 Only\)

| Property | Description |
| :--- | :--- |
| App Name | Name of the app as it appears below the icon on the phone. Will be set to the project name initially. |
| Icon | App icon -- the recommended app icon size is 150 px by 150 px |
| About Screen | Appears when "About this Application" is selected from the system menu. The title must be visible for this screen to be visible |
| Sizing | If set to responsive \(recommended\), screen layouts will autoscale to the size of the screen. Components should be sized to 'percent' height and width. If set to fixed, screen layouts will be created for a single fixed-sized screen and components should be sized to 'pixels' height and width |
| Version Name | Description which helps users distinguish between different versions of your app on the Google Play Store |
| Version Code | An integer value which must be incremented each time a new .apk is created for the Google Play Store |
| Theme | Specifies the look and feel of Material Design user interface elements such as buttons and title bars. App theme options include `Classic` \(default\), `Device Default`, `Black Title Text` and `Dark` |
| Primary Color | Specifies the primary color for Material Design user interface elements such as buttons and title bars |
| Primary Color Dark | Specifies the primary dark color for Material Design user interface elements such as buttons and title bars |

### Appearance

| Property | Description |
| :--- | :--- |
| Title | Displayed on title bar |
| Title Visible | If checked, shows a default \(gray\) title bar on the screen |
| Show Status Bar | If checked, shows the top most bar on the screen which displays time, battery etc |
| Alight Horizontal | Center, Left or Right |
| Alight Vertical | Center, Top or Bottom |
| Background Image | You can upload an image to your app or reference an image url |
| Background Color | Default \(White\). You can choose any color on the Designer palette or customize the color to any RGB value in the Blocks editor |
| Scrollable | If checked, there will be a vertical scrollbar on the screen. If unchecked, the app height is limited to the height of the device |
| Screen Orientation | Unspecified \(default\), Portrait, Landscape, Sensor and User |
| Open Screen Animation | Default, Fade, Zoom, Slide Horizontal, Slide Vertical and None |
| Close Screen Animation | Default, Fade, Zoom, Slide Horizontal, Slide Vertical and None |

### Functionality

| Event | Description |
| :--- | :--- |
| Initialize | If Screen1, starts all events when the app is open. If another screen, starts all events when that screen is open |
| Back Pressed | When the device's back button is pressed |
| Other Screen Closed \(otherScreenName, result\) | When another screen has closed and control has returned to this screen |
| Error Occurred \(component, functionName, errorNumber, message\) | When an error occurs -- only some errors will trigger this event |
| Screen Orientation Changed | When screen orientation changes |

