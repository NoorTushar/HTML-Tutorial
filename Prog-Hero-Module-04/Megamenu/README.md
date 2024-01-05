### Megamenu

When you use the CSS selector `nav li .dropdown`, it will select only those`li`items which has `dropdown` class inside them.

```html
<header>
  <h2 style="text-align: center; margin: 20px 0">Semantic Markups</h2>
  <nav>
    <ul>
      <li><a href="index.html">Home</a></li>
      <li><a href="audio-video.html">Audio/Video</a></li>
      <li><a href="employee-table.html">Employees</a></li>
      <li><a href="semantic-html5.html">Semantic-Markups</a></li>
      <li>
        <a href="pitha-form.html">Pitha Form</a>
        <ul class="dropdown">
          <li><a href="index.html">Home</a></li>
          <li><a href="audio-video.html">Audio/Video</a></li>
          <li>
            <a href="employee-table.html">Employees</a>
            <ul class="dropdown">
              <li><a href="index.html">Home</a></li>
              <li><a href="audio-video.html">Audio/Video</a></li>
              <li><a href="employee-table.html">Employees</a></li>
              <li>
                <a href="semantic-html5.html">Semantic-Markups</a>
                <ul class="dropdown">
                  <li><a href="index.html">Home</a></li>
                  <li><a href="audio-video.html">Audio/Video</a></li>
                  <li><a href="employee-table.html">Employees</a></li>
                  <li>
                    <a href="semantic-html5.html">Semantic-Markups</a>
                  </li>
                </ul>
              </li>
            </ul>
          </li>
          <li>
            <a href="semantic-html5.html">Semantic-Markups</a>
          </li>
        </ul>
      </li>
    </ul>
  </nav>
</header>
<script>
  document.querySelectorAll("a").forEach((a) => {
    console.log((a.href = "#"));
  });
</script>
```

```css
header {
  margin: 10px 0;
}
nav > ul {
  display: flex;
  justify-content: center;
  gap: 25px;
}
nav ul li a {
  color: black;
}

/* Mega-menu Styles Start from here*/

/* here it will select the ul which has the class 'dropdown' inside a li */
nav li .dropdown {
  margin-left: 15px;
  position: absolute;
  background-color: white;
  display: none;
}

/* here is the trick, you will first of all hover the li which has the class .dropdown inside it, it then the immediate child will be displayed block and not all the dropdown elements */
nav li:hover > .dropdown {
  display: block;
}

/* it will give padding to all the list items which has the dropdown class */
nav li .dropdown li {
  padding: 5px;
}
```

Output: 3 layers of inside menu, mega menu.

![Alt text](image.png)
