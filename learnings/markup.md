# Agency website project

### Main goal of the project 

In this [project](https://cazanelena.github.io/agency-website/), our goal was to create an agency website with a strong focus on accessibility. The main requirements of the site were centered around utilizing semantic HTML to enhance accessibility, ensuring optimal readability for screen readers, and achieving sufficient color contrast in the UI to ensure comfortable perception for all users. To ensure compliance with accessibility standards, we utilized a variety of tools to thoroughly assess our website's accessibility criteria.
[Here](https://github.com/cazanelena/agency-website) is the GitHub repo.  


## 1. Structure a site using semantic HTML to aid accessibility

Using semantic HTML to structure your site not only aids accessibility by improving the experience for screen readers and users with disabilities but also enhances SEO, provides consistent styling and behavior, future-proofs your website, and expands your audience reach. It is an essential practice for creating accessible and well-optimized web content.

```html
    <nav>
      <ul id="navList" class="row justify-end">
        <li>
          <a href="#about">About</a>
        </li>
        <li>
          <a href="#contact">Contact</a>
        </li>
      </ul>
```
The code snippet above uses <nav> elements that we used to create a nav bar. Screen readers rely on HTML semantics to understand and convey the content of a web page to users with visual impairments. By using semantic HTML elements such as ```<header>, <nav>, <main>, <section>, <article>, and <footer>```, you provide a clear structure and meaning to the content, enabling screen readers to navigate and present the information accurately.
  
## 2. Ensure a web page is readable for screen readers
  
  ```html
  <img src="Images/teamwork.png" alt="teamwork image" /> // Tells the user what the image contains 
        <h3>Collaborate with us</h3>
  ```
Providing Alternative Text for Images: We added descriptive alternative text (alt text) to images using the alt attribute. The alt text should convey the meaning or purpose of the image to users who cannot see it.

## 3. Ensure our UI has sufficient colour contrast so that everyone can perceive it comfortably
  
There are numerous tools available to assist you in selecting the perfect color scheme for your website. After establishing a solid structure for our site, we utilized a reliable color generator, such as [Colors](https://coolors.co/), to ensure a well-balanced contrast. This allowed us to fine-tune our color choices and achieve an appealing visual harmony on our web pages.
  
## 4. Use various tools to check that our website meets accessibility criteria

  For this project we used lighthouse. This is an open-source tool developed by Google that can audit web pages for performance, accessibility, SEO, and more. It is available as a feature in the Chrome DevTools or as a browser extension. 
    
![](learnings/accessibility1.png)
![](learnings/accessibility2.png)
![](learnings/accessibility3.png)

## 5. Use CSS media queries to ensure our content is always presented effectively on screens of different sizes
  
We made effective use of flexbox, leveraging its capabilities to ensure our website's responsiveness across various devices. In addition, we incorporated media queries to further enhance the adaptability of our design. By employing these techniques, we were able to create a visually appealing and user-friendly experience that seamlessly adjusts to different screen sizes and orientations.
    
```css
@media screen and (max-width: 1024px) {

  html {
    overflow-x: hidden;
  }

  body {
    overflow-x: hidden;
  }

  .change-bg{
    overflow-x: hidden;
  }
  .column {
    display: flex;
    flex-direction: column;
    justify-content: center;  
    align-items: center;
    }
}
``` 
    
## 6. Demonstrate a mobile-first approach to building a website
    
Responsive design: We implemented responsive design techniques using CSS media queries. Started by designing and styling the mobile layout first, ensuring that the site looks and functions well on smaller screens. Gradually add breakpoints and adjust the layout for larger screen sizes, such as tablets and desktops.

Progressive enhancement: We employed progressive enhancement to ensure that essential content and functionality are available on all devices. Started with a solid foundation of HTML and CSS that worked across all platforms and progressively enhanced the experience by adding more advanced features for larger screens.

Viewport meta tag: We included the viewport meta tag in the <head> section of your HTML document. This tag helps ensure that the website adapts to the device's screen size and sets the initial scale appropriately for mobile devices.

```html
    <!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta
      name="viewport"
      content="width=device-width, initial-scale=1, minimum-scale=1"
    />
    <title>Agency website</title>
```
     


## 7. Use CSS Flexbox to style children in a single-direction layout (ie a row or a column)
```css
      
.row {
  display: flex;
  flex-wrap: wrap;
  gap: 2.5rem;
  align-items: center;
}

.stretch {
  align-items: stretch;
}

.col {
  display: flex;
  flex-direction: column;
}

.justify-end {
    justify-content: flex-end;
}
```
CSS Flexbox is a powerful layout module that provides a flexible way to arrange and align elements within a container such as a rows and columns. It offers a simple and intuitive approach to building responsive and dynamic layouts.
      

## 8. Ensure our Git commit history tells a coherent story
      
Maintaining a coherent Git commit history is essential for effective collaboration and project management. 
We made sure the commit messages were clear and descriptive that succinctly summarize the changes made in the commit. The commit should have a meaningful message that provided context and explained the purpose of the changes.


## 9. Use the appropriate input types in HTML forms for gathering different types of information
