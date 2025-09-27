# Breadcrumb Component
# Youtube Video Step by step demo
🔗https://youtu.be/sEzmuXWuvjs

## 📥 How to Use
1. Download `BreadcrumbComponent.msapp`
2. Open PowerApps Studio → Your App
3. Go to Tree View → Components → Import
4. Select the file and import
5. Drag the component into your screen and configure
6. Update below code on Home Screen – OnVisible(): 
ClearCollect(
    colScreenDetails,
    Table(
        {
            Screen: '<Your home scree name>',
            Count: 1
        }
    )
);

Update below code on Other Screens OnVisible():
If(
    IsBlank(
        LookUp(
            colScreenDetails,
            Screen = App.ActiveScreen
        )
    ),
    Collect(
        colScreenDetails,
        {
            Screen: App.ActiveScreen,
            Count: CountRows(colScreenDetails) + 1
        }
    )
);

# Header Component
Reusable header layout with logo, app title, and navigation buttons—all driven by a single config object.

📥 How to Use
Download HeaderComponent.msapp

Open PowerApps Studio → Your App

Go to Tree View → Components → Import

Select the file and import

Drag the component into your screen

Set the component’s HeaderConfig property using the structure below

⚙️ Configuration via HeaderConfig
Use the following schema to define your header layout. This drives logo, title, and navigation buttons—no additional properties required.

powerfx
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

