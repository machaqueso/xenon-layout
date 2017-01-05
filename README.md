# xenon-layout

`<xenon-layout>` provides simple responsive page layout. Use the special children elements 
`<header>`, `<nav>`, `<main>`, and `<footer>` to layout the page. Inside the nav element, the 
`<nav-item>` element can be used to make navigation links. 

## Example:
    <style is="custom-style">
        :root { --xenon-layout-background-color:purple; --xenon-layout-color:white; }
    </style>
    <xenon-layout title-text="This Is A Test">
        <header><iron-icon icon="add-circle"></iron-icon></header>
        <nav style="display:flex; flex-direction:column;">
            <nav-item icon="settings">Menu Item One</nav-item>    
            <nav-item icon="add">Menu Item Two</nav-item>    
            <nav-item icon="cancel">Menu Item Three</nav-item>  
            <div style="flex: 1 1 auto"></div>
            <div style="align-self:center;">bottom logo here</div>  
        </nav>
        <main style="max-width:1200px;">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. 
        </main>
        <footer style="text-align:right">hello footer</footer>
    </xenon-layout>
