# HTML Tutorials by Noor Tushar - Module 04

### Semantic HTML

```html
<body>
  <header>
    <nav>
      <ul>
        <li><a></a></li>
        <li><a></a></li>
        <li><a></a></li>
      </ul>
    </nav>
  </header>
  <main>
    <article>
      <header>
        <!-- Contains title and also time usually -->
        <time datetime=""></time>
      </header>
      <figure>
        <img src="" />
        <figcaption></figcaption>
      </figure>
      <section>
        <!-- first section -->
      </section>
      <section>
        <!-- second section -->
      </section>
      <section>
        <!-- third section -->
      </section>
      <footer>
        <!-- might contain tag links -->
      </footer>
    </article>
  </main>
  <footer>
    <!-- Footer Section -->
  </footer>
</body>
```

### Form

```html
<body>
  <header>
    <nav>
      <ul>
        <li><a href="index.html">Home</a></li>
      </ul>
    </nav>
  </header>
  <main>
    <section class="form-section">
      <form>
        <h2>Sokhina Khala Pitha Ghor</h2>
        <!-- name field -->
        <label for="name"
          >Your Name:
          <input type="text" name="name" id="name" placeholder="Your Name"
        /></label>
        <!-- email field -->
        <label for="email"
          >Your Email:
          <input type="email" name="email" id="email" placeholder="Your Email"
        /></label>
        <!-- phone field -->
        <label for="phone"
          >Your Phone:
          <input type="text" name="name" id="phone" placeholder="Your Phone"
        /></label>

        <fieldset class="pitha">
          <legend>Chose any <b>one</b> pitha</legend>
          <label for="bhapa">
            <input type="radio" name="pitha" id="bhapa" />Bhapa</label
          >
          <label for="chitoi">
            <input type="radio" name="pitha" id="chitoi" />Chitoi</label
          >
          <label for="kuli">
            <input type="radio" name="pitha" id="kuli" />Kuli</label
          >
        </fieldset>

        <fieldset class="bhorta">
          <legend>Chose your bhortas</legend>
          <label for="shukti"
            ><input type="checkbox" name="shutki" id="shutki" />Shutki</label
          >
          <label for="alu"
            ><input type="checkbox" name="alu" id="alu" />Alu</label
          >
          <label for="begun"
            ><input type="checkbox" name="begun" id="begun" />Begun</label
          >
        </fieldset>

        <fieldset class="instruction">
          <legend>Give your instructions</legend>
          <textarea name="instruction" id="instruction" rows="5"></textarea>
        </fieldset>
      </form>
    </section>
  </main>
  <footer></footer>
</body>
```

### Table

```html
<body>
  <header>
    <nav>
      <ul>
        <li><a href="index.html">Home</a></li>
      </ul>
    </nav>
  </header>
  <main>
    <section class="employee-section">
      <h2>Employee Table</h2>
      <table>
        <caption>
          Employee Salary Table
        </caption>
        <thead>
          <th>Sl.No</th>
          <th>Employee Name</th>
          <th>Department</th>
          <th>Salary</th>
        </thead>
        <tbody>
          <tr>
            <td>1</td>
            <td>Alex</td>
            <td>Marketing</td>
            <td>BDT 10,000</td>
          </tr>
          <tr>
            <td>2</td>
            <td>Mark</td>
            <td>Operations</td>
            <td>BDT 20,000</td>
          </tr>
          <tr>
            <td>3</td>
            <td>Tim</td>
            <td>Finance</td>
            <td>BDT 30,000</td>
          </tr>
        </tbody>
        <tfoot>
          <tr>
            <td colspan="4"><b>Total Employees: 3</b></td>
          </tr>
        </tfoot>
      </table>
    </section>
  </main>
  <footer></footer>
</body>
```
