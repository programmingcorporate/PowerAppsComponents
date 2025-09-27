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


