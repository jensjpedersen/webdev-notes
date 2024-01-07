
# React router

**Key concepts:**
* <Link> - creates a link to another page in the app. It is used instead of <a href="">.
* <Outlet> - Specify where the child routes should be rendered. It's like a
  placeholder for the content of nested routes. 
* <BrowserRouter> - Wrapper component that provides the routing functionality.
  Should be used once in the app.
* <Routes> - Used to define the routes of the app. It should be used inside
  <BrowserRouter>. Contains a list of <Route> components.
* <Route> - defines a single route:
    * special props: *, index



## Installation
```bash
npm i -D react-router-dom
```


## Structure 
```
src\pages\:

Layout.js
Home.js
Blogs.js
Contact.js
NoPage.js
```

## Basic Usage
```javascript

import { BrowserRouter, Routes, Route } from "react-router-dom";

export default function App() {
  return (
    <BrowserRouter>
      <Routes>
        <Route path="/" element={<Layout />}>
          <Route index element={<Home />} />
          <Route path="blogs" element={<Blogs />} />
          <Route path="contact" element={<Contact />} />
          <Route path="*" element={<NoPage />} />
        </Route>
      </Routes>
    </BrowserRouter>
  );
}
```


## Special routes
```
* - catch all undefined routes
```


# Special components
## Layout route 
* The "layout route" is a shared component that inserts common content on all
pages, such as a navigation menu.

* Anytime we link to an internal path, we will use <Link> instead of <a href="">.


**Elements**
* <Link> - creates a link to another page in the app
* <Outlet> - renders the current route selected 

### Template
```javascript
import { Outlet, Link } from "react-router-dom";

const Layout = () => {
  return (
    <>
      <nav>
        <ul>
          <li>
            <Link to="/">Home</Link>
          </li>
          <li>
            <Link to="/blogs">Blogs</Link>
          </li>
          <li>
            <Link to="/contact">Contact</Link>
          </li>
        </ul>
      </nav>

      <Outlet />
    </>
  )
};

export default Layout;

```

