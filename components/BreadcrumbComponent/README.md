# Breadcrumb Component

## 📥 How to Use
1. Download `BreadcrumbComponent.msapp`
2. Open PowerApps Studio → Your App
3. Go to Tree View → Components → Import
4. Select the file and import
5. Drag the component into your screen and configure
6. Update below code on Home Screen – OnVisible
// Initialize breadcrumb trail with the Home screen
ClearCollect(
    colScreenDetails,
    Table(
        {
            Screen: '<Your home scree name>',
            Count: 1
        }
    )
);

Update below code on Other Screens OnVisible
// Add current screen to breadcrumb trail if not already present
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

