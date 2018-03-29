# UWPFullScreenAcrylicApp
Sample to show Full Screen Acrylic App appearance

I noticed that on UWP, That background Window Acrylic effect does not work on a Page started at Full screen. Only after you restore it, the effect appears. Can you check this?

When start in Full Screen it seems that Acrylic effect is not drawn; Then try to restore the window, you will notice that the Acrylic effect works.



I Enabled it using

        public App()
        {
            Windows.UI.ViewManagement.ApplicationView.PreferredLaunchWindowingMode =
                Windows.UI.ViewManagement.ApplicationViewWindowingMode.FullScreen
                ;

            this.InitializeComponent();
            this.Suspending += OnSuspending;
        } 
        
and on the page:

<Page
    x:Class="FullScreenAcrylicApp.MainPage"
    xmlns="http://schemas.microsoft.com/winfx/2006/xaml/presentation"
    xmlns:x="http://schemas.microsoft.com/winfx/2006/xaml"
    xmlns:local="using:FullScreenAcrylicApp"
    xmlns:d="http://schemas.microsoft.com/expression/blend/2008"
    xmlns:mc="http://schemas.openxmlformats.org/markup-compatibility/2006"
    mc:Ignorable="d"
    Background="{StaticResource SystemControlAcrylicWindowBrush}">

    <Grid>
        <TextBlock>HELLO WORLD. 
            Check if the Acrylic Background is working.
            Restore window, maximize it.
        </TextBlock>

    </Grid>
</Page>
