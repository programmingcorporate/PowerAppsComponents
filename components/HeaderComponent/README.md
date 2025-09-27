
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

```powerfx
Table(
    {
        // Header background styling
        Type: "HeaderBackground",
        HeaderBackground: Color.LightGray,
        HeaderDropShadow: "Heavy"
    },
    {
        // Logo image
        Type: "Image",
        Image: 'CompanyLogo',
        ImageSize: 50,
        ImageType: 1
    },
    {
        // App title text
        Type: "Text",
        AppName: "Title Of App",
        TextWeight: "Bold",
        FontSize: 15,
        FontType: Font.'Segoe UI',
        Align: "Center",
        FontColor: Color.DarkBlue
    },
    {
        // Navigation button 1
        Type: "Button",
        Label: "Home",
        ScreenName: 'Home',
        Icon: "Home",
        IconStyle: "Filled",
        IconPosition: "Start",
        ButtonType: "Primary",
        BackgroundColor: RGBA(0, 0, 1, 1)
    },
    {
        // Navigation button 2
        Type: "Button",
        Label: "Screen2",
        ScreenName: 'Screen2',
        Icon: "Add",
        IconStyle: "Outline",
        IconPosition: "Only",
        ButtonType: "Primary",
        BackgroundColor: Color.Red
    },
    {
        // Navigation button 3
        Type: "Button",
        Label: "Screen3",
        ScreenName: 'Screen3',
        Icon: Blank(),
        IconStyle: Blank(),
        IconPosition: Blank(),
        ButtonType: "Primary",
        BackgroundColor: Color.Blue
    }
)




🧭 Notes
All layout, styling, and navigation logic is driven by HeaderConfig

No need to modify the component directly—just update the config

Supports dynamic schema: add/remove buttons, change styles, or localize labels
