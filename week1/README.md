## Creating a Webpage from a Figma Design



<details><summary>Figma Design (https://www.figma.com/file/77OFKcKrEwPd7YxZndxett/Happy-Dog-Cafe?node-id=0%3A1)</summary>

![Screen Shot 2022-09-24 at 2 14 59 PM](https://user-images.githubusercontent.com/54293301/192155990-650f253b-98a4-4797-8cfd-41c55152f5f6.png)

</details>


You can clone this project and play around with the files

### Creating HTML file


Generate a template by typing `html:5` and hitting tab on the keyboard or selecting it
<details><summary>Demo</summary>


https://user-images.githubusercontent.com/54293301/192156022-decc3937-18d9-4131-a6b9-99510c3b17fe.mov


</details>


#### Using semantic HTML

There are many [elements](https://developer.mozilla.org/en-US/docs/Web/HTML/Element) that are available when building an HTML page.

Try to use [semantic HTML](https://developer.mozilla.org/en-US/docs/Glossary/Semantics) when possible. There is no visual difference but it helps to add some more meaning to components on the page. It also increases the accessibility for the visually impaired using screen readers.

For example, using `<strong>` instead of `<br>` and when you're creating a list of items, using `<li>` and `<ul> or <ol>` instead of `<div>`

#### Importing fonts

Google has a resource for fonts that can be easily used [https://fonts.google.com/](https://fonts.google.com/)

Fonts are imported in the `<head>` of the html file

#### Spacing: Margin/Padding

There are two styling properties that can add spacing <strong>margin</strong> and <strong>padding</strong>
Margin is spacing added <strong>outside</strong> the element, while padding is adding it <strong>inside</strong>

<details><summary>demo video</summary>

 https://user-images.githubusercontent.com/54293301/192155964-f330fbf3-0de1-4ed6-a2c3-755a7310bb8c.mov
</details>


#### Layout Methods

[Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)

Alternatively, you can also use [grid](https://css-tricks.com/snippets/css/complete-guide-grid/)

> <strong>Flexbox</strong> is one-dimensional, while CSS Grid is two-dimensional. Flexbox lays out items along either the horizontal or the vertical axis, so you have to decide whether you want a row-based or a column-based layout.
>
> On the other hand, <strong>CSS Grid</strong> lets you work along two axes: horizontally and vertically. Grid allows you to create two-dimensional layouts where you can precisely place grid items into cells defined by rows and columns.

#### Devtools

to play around with the DOM, elements on the webpage
Right click and Inspect

#### Adding images

- get the url from the web
```javascript
<img src="https://post.medicalnewstoday.com/wp-content/uploads/sites/3/2020/02/322868_1100-800x825.jpg" />
```

- download image into project and specify the path in the src attribute
```javascript
<img src="assets/dog.png" />
```

#### Responsiveness

- Good practice is to design for smaller devices first and then desktop

![Screen Shot 2022-09-25 at 1 09 49 PM](https://user-images.githubusercontent.com/54293301/192156152-c8bb37b7-b109-452b-9db0-ea177b68cef7.png)

This is the syntax, it consists of 4 parts
1. @media Rule which indicates that it's a media query
2. the [media type](https://developer.mozilla.org/en-US/docs/Web/CSS/@media#media_types) -> screen
3. the [operator](https://developer.mozilla.org/en-US/docs/Web/CSS/@media#media_types) -> and
4. the feature (the environment you're applying the specific styles to) -> (min-width: 468px)

```javascript
@media screen and (min-width: 468px) {
  h1 {
    color: yellow;
    text-align: center;
  }
}
```
#### Final notes

- Google will usually have solutions when you find your self stuck, you just gotta know the right questions to ask it
- Use the devTools, it will allow you to manipulate and play around with the html and css without applying any code
- There is a lot of information out there, and a good way to start learning is to start building something!
