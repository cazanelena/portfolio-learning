# Agency website project

### Main goal of the project 

In this project, our goal was to create an agency website with a strong focus on accessibility. The main requirements of the site were centered around utilizing semantic HTML to enhance accessibility, ensuring optimal readability for screen readers, and achieving sufficient color contrast in the UI to ensure comfortable perception for all users. To ensure compliance with accessibility standards, we utilized a variety of tools to thoroughly assess our website's accessibility criteria.


## 1. Structure a site using semantic HTML to aid accessibility

Using semantic HTML to structure your site not only aids accessibility by improving the experience for screen readers and users with disabilities but also enhances SEO, provides consistent styling and behavior, future-proofs your website, and expands your audience reach. It is an essential practice for creating accessible and well-optimized web content.

```
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
The code snippet above uses <nav> elements that we used to create a nav bar. Screen readers rely on HTML semantics to understand and convey the content of a web page to users with visual impairments. By using semantic HTML elements such as <header>, <nav>, <main>, <section>, <article>, and <footer>, you provide a clear structure and meaning to the content, enabling screen readers to navigate and present the information accurately.
  
## 2. Ensure a web page is readable for screen readers
  
  ```
  <img src="Images/teamwork.png" alt="teamwork image" /> // Tells the user what the image contains 
        <h3>Collaborate with us</h3>
  ```
Providing Alternative Text for Images: We added descriptive alternative text (alt text) to images using the alt attribute. The alt text should convey the meaning or purpose of the image to users who cannot see it.

## 3. Ensure our UI has sufficient colour contrast so that everyone can perceive it comfortably
  
There are numerous tools available to assist you in selecting the perfect color scheme for your website. After establishing a solid structure for our site, we utilized a reliable color generator, such as [Coolors](https://coolors.co/), to ensure a well-balanced contrast. This allowed us to fine-tune our color choices and achieve an appealing visual harmony on our web pages.
  
## 4. Use various tools to check that our website meets accessibility criteria

  For this project we used lighthouse. This is an open-source tool developed by Google that can audit web pages for performance, accessibility, SEO, and more. It is available as a feature in the Chrome DevTools or as a browser extension. 

## 5. Use CSS media queries to ensure our content is always presented effectively on screens of different sizes
  We made a good use of the flexbox and this help us in making sure the website was 

## 6. Demonstrate a mobile-first approach to building a website

## 7. Use CSS variables to apply repeated colours to HTML elements

## 8. Use CSS Flexbox to style children in a single-direction layout (ie a row or a column)

## 9. Use CSS Grid to style children in two-direction layout

## 10. Ensure our Git commit history tells a coherent story

## 11. Use the appropriate input types in HTML forms for gathering different types of information
