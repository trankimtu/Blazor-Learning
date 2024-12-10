# Blazor-Learning

## Multiple  startup project
<ul>
  <li>Right click Soulution</li>
  <li>Select Configure Startup Project</li>
  <li>Under Common Properties > Startup Project</li>
  <li>Check multiple startup projects:</li>
  <li>Set Action = "start"</li>
  <li></li>
</ul>

# BankofWhittier
## Files Structure
<ul>
  <li>Root Directory</li>
  <li>
    Components
    <ul>
      <li>Button</li>
      <li>Card</li>
      <li>LoginForm</li>
    </ul>
  </li>
  
  <li>
    Layouts
    <ul>
      <li>MainLayout</li>
      <li>HomeLayout</li>
      <li>FormLayout</li>
      <li>AdminLayout</li>
    </ul>
  </li>
  
  <li>
    Pages
    <ul>
      <li>Home</li>
      <li>About</li>
      <li>Contact</li>
      <li>
        Forms
        <ul>
          <li>FormPage1</li>
          <li>FormPage2</li>
        </ul>
      </li>
    </ul>
  </li>
  
  <li>
    Shared
    <ul>
      <li>DataService.cs</li>
      <li>custom.css</li>
      <li>Footer</li>
      <li>Header</li>
    </ul>
  </li>
  <li>
    wwwroot
    <ul>
      <li>css</li>
      <li>images</li>
      <li>js</li>
    </ul>
  </li>
</ul>

Ex:
```
<!-- HomeLayout.razor -->
@inherits LayoutComponentBase

<div class="home-layout">
    <header>
        <h1>Home Page</h1>
    </header>
    <main>
        @Body
    </main>
    <footer>
        <p>&copy; 2024 Home Page</p>
    </footer>
</div>

```
```
<!-- Home.razor -->
@page "/home"
@layout HomeLayout

<h2>Welcome to the Home Page</h2>
<p>This is the home page content.</p>
```
```
<!-- _Imports.razor -->
@using BlazorServer.Layouts

```
