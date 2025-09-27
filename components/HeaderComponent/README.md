
# Header Component
Reusable header layout with logo, app title, and navigation buttons—all driven by a single config object.

<img width="1125" height="62" alt="image" src="https://github.com/user-attachments/assets/bb916810-25c0-4e6b-abca-76e7a1679252" />


📥 How to Use
CanvasHeaderComponents.msapp

Open PowerApps Studio → Your App

Go to Tree View → Components → Import

Select the file and import

Drag the component into your screen

Set the component’s HeaderConfig property using the structure below

⚙️ Configuration via HeaderConfig
Use the following schema to define your header layout. This drives logo, title, and navigation buttons—no additional properties required.

# NOTE: Add or Remove buttons from Table() based on business requirement 
```powerfx
Table(
    {
        // Header background configuration
        Type: "HeaderBackground",               // Defines overall header styling
        HeaderBackground: Color.LightGray,      // Background color for the header container
        HeaderDropShadow: DropShadow.Bold
    },
    {
        // Image control configuration
        Type: "Image",                          // Control type: "Image"
        Image: 'CompanyLogo',                   // Media reference (e.g., uploaded image or media name)
        ImageSize: 50                         // Image size in pixels
   
    },
    {
        // Text control configuration
        Type: "Text",                           // Control type: "Text" (used for labels, headers, captions)
        AppName: "App Title",                // Display text for the app title
        TextWeight: "Bold",                     // Text weight: "Bold" or "Normal"
        FontSize: 20,                           // Font size in points (e.g., 12, 14, 16, 20)
        FontType: Font.'Segoe UI',              // Font family (e.g., "Segoe UI", "Arial", "Calibri")
        Align: "Center",                        // Text alignment: "Left", "Center", "Right"
        FontColor: Color.DarkBlue               // Text color
    },
    {
        // Button 1 configuration
        Type: "Button",                         // Control type: "Button"
        Label: "Home",                          // Display text
        ScreenName: 'Home',                     // Target screen to navigate
        Icon: "Home",                           // Fluent icon name (e.g., "Home", "Add", "Flight")
        IconStyle: "Filled",                    // Icon style: "Filled" or "Outline"
        IconPosition: "Start",                  // Icon placement: "Start", "End", "Only"
        ButtonType: "Primary",                  // Appearance: "Primary", "Secondary", "Subtle", "Transparent"
        BackgroundColor: RGBA(0, 0, 1, 1)       // Background color (can use Color.X or RGBA)
    },
    {
        // Button 2 configuration
        Type: "Button",
        Label: "Screen2",                       //Replace with your screen name
        ScreenName: 'Screen2',                  //Replace with your screen name
        Icon: "Add",                            // Icon-only button
        IconStyle: "Outline",
        IconPosition: "Only",                   // Icon-only display
        ButtonType: "Primary",                  // Appearance: "Primary", "Secondary", "Subtle", "Transparent"
        BackgroundColor: Color.Red              // Background color
    },
    {
        // Button 3 configuration
        Type: "Button",
        Label: "Screen3",
        ScreenName: 'Screen3',
        Icon: Blank(),                          // No icon
        IconStyle: Blank(),                     // No style applied
        IconPosition: Blank(),                  // No icon position
        ButtonType: "Primary",                  // Appearance: "Primary", "Secondary", "Subtle", "Transparent"
        BackgroundColor: Color.Blue             // Background color
    }
)


🧭 Notes
All layout, styling, and navigation logic is driven by HeaderConfig

No need to modify the component directly—just update the config

Supports dynamic schema: add/remove buttons, change styles, or localize labels
