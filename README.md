
# CSS Workshop Outline

## 1. Implementing CSS
- **[Inline](https://www.w3schools.com/css/css_howto.asp) CSS**
  - Change text [`color`](https://developer.mozilla.org/en-US/docs/Web/CSS/color) for `<h1>` with inline CSS.

- **[Internal](https://www.w3schools.com/css/css_howto.asp) CSS**
  - Change [`background-color`](https://developer.mozilla.org/en-US/docs/Web/CSS/background-color) for `<h1>` with internal CSS.
- **[External](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/link) CSS File**
  - Remove inline and internal CSS.
  - Create a **new general** `general.css` file in `/Styles` folder.
  - Link this CSS file in every HTML file.
 - **Reset Default Styles in general CSS**
   - Resetting default margins and paddings for common elements to ensure consistency and set default font for text:
    ```css
    body, h1, h2, h3, p, ul, li, nav, section, article, footer {
        margin: 0;
        padding: 0;
    }

    body {
       font-family: 'Arial', sans-serif; /* Sets the font across the whole page */
    }
    ```

## 2. Styling Elements
### 2.1 Edit `<h2>`
- Change [`color`](https://developer.mozilla.org/en-US/docs/Web/CSS/color) to blue (`#134169`).
- Set [`font-weight`](https://developer.mozilla.org/en-US/docs/Web/CSS/font-weight) to 600.
- Add [`border-bottom: 2px solid #1f8dc8`](https://developer.mozilla.org/en-US/docs/Web/CSS/border-bottom).

### 2.2 Edit Paragraph
- Change [`color`](https://developer.mozilla.org/en-US/docs/Web/CSS/color) to `#555`.
- Set [`text-align`](https://developer.mozilla.org/en-US/docs/Web/CSS/text-align) to justify.
- Set [`line-height`](https://developer.mozilla.org/en-US/docs/Web/CSS/line-height) to 1.8.


## 3. About Us CSS File
- Add a new CSS file with name `about.css` for the **"About Us"** page.
- [Link](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/link) the **"About Us"** CSS file with HTML file.

## 4. Style for ID Selector "About"
- Add [`id="about"`](https://developer.mozilla.org/en-US/docs/Web/CSS/ID_selectors#examples) value to the **first** `<section>` element in **"About Us"** HTML.
- Create "About" ID selector in the **"About Us"** CSS file.
  - Change [`background-color`](https://developer.mozilla.org/en-US/docs/Web/CSS/background-color) (recommend LightGrey).
  - Set [`max-width`](https://developer.mozilla.org/en-US/docs/Web/CSS/max-width) of the section to 85vw.
  - Optional: Change [`font-size`](https://developer.mozilla.org/en-US/docs/Web/CSS/font-size) to 110%.

## 5. [Box Model](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/The_box_model#what_is_the_css_box_model) for ID Selector "About"
- Add a red [`border`](https://developer.mozilla.org/en-US/docs/Web/CSS/border) around whole section.
- Margin: Center the section 
  - `margin-top` and `margin-bottom` to 20px.
  -  `margin-left` and `margin-right` to auto.
  -  [`border-radius`](https://developer.mozilla.org/en-US/docs/Web/CSS/border-radius) to 16px.
  - Optional: Use **shorthand** - [`margin: 20px auto`](https://developer.mozilla.org/en-US/docs/Web/CSS/margin).
- Padding: Set [`padding`](https://developer.mozilla.org/en-US/docs/Web/CSS/padding) to 40px for all sides of section.
- *Remove the red border afterwards.*

## 6. Edit `<h3>` in GENERAL CSS
- Set [`color`](https://developer.mozilla.org/en-US/docs/Web/CSS/color) and [`text-align`](https://developer.mozilla.org/en-US/docs/Web/CSS/text-align).
- Edit box model: 
  - Set [`margin`](https://developer.mozilla.org/en-US/docs/Web/CSS/margin), [`padding`](https://developer.mozilla.org/en-US/docs/Web/CSS/padding), and a screen-wide [`border-bottom`](https://developer.mozilla.org/en-US/docs/Web/CSS/border-bottom).

## 7. Team Member Divisions
### 7.1 Individual Divisions
- Create a HTML `<div>` for each team member 
  - **Team member** consists of **image**, **name** and **description**
- Assign [`class="team-member"`](https://developer.mozilla.org/en-US/docs/Web/CSS/Class_selectors) to each `<div>`.
- In `about.css` CSS, set [`margin`](https://developer.mozilla.org/en-US/docs/Web/CSS/margin), [`padding`](https://developer.mozilla.org/en-US/docs/Web/CSS/padding), [`border`](https://developer.mozilla.org/en-US/docs/Web/CSS/border), [`border-radius`](https://developer.mozilla.org/en-US/docs/Web/CSS/border-radius), and [`background-color`](https://developer.mozilla.org/en-US/docs/Web/CSS/background-color) in `team-member` class.
- Set [`width`](https://developer.mozilla.org/en-US/docs/Web/CSS/width) to 20vw and [`height`](https://developer.mozilla.org/en-US/docs/Web/CSS/height) to auto in `team-member`.

### 7.2 Team Member Container
- Create a new `<div>` under **"Meet Our Team"** `<h3>` which will contain all team member **divs**.
- In HTML set an [ID selector](https://developer.mozilla.org/en-US/docs/Web/CSS/ID_selectors) for this `<div>`  and add it to the **"About Us"** CSS file.
- Add these properties to newly created [ID selector](https://developer.mozilla.org/en-US/docs/Web/CSS/ID_selectors)
  ```css
    display: flex; /* Enables flexbox layout */
    flex-wrap: nowrap; /* Doesn't allows items to wrap to new lines*/
    justify-content: space-around; /* Distributes space around items */
    align-items: flex-start; /* Aligns items to the start of the flex container */
   ```

  - [``display:  flex``](https://developer.mozilla.org/en-US/docs/Web/CSS/display) 
  - [``flex-wrap:  nowrap``](https://developer.mozilla.org/en-US/docs/Web/CSS/flex-wrap)
  - [``justify-content:  space-around``](https://developer.mozilla.org/en-US/docs/Web/CSS/justify-content)
  - [``align-items:  flex-start``](https://developer.mozilla.org/en-US/docs/Web/CSS/align-items)

## 8. Style for Team Member Images
- Create a [descendant *(combinator)* selector](https://developer.mozilla.org/en-US/docs/Web/CSS/Descendant_combinator) for `img` *(images)* under the `team-member` class.
  - Set [`width`](https://developer.mozilla.org/en-US/docs/Web/CSS/width) to 100%, [`height`](https://developer.mozilla.org/en-US/docs/Web/CSS/height) to auto.
  - Optional: Set [`border-radius`](https://developer.mozilla.org/en-US/docs/Web/CSS/border-radius), [`margin`](https://developer.mozilla.org/en-US/docs/Web/CSS/padding), and [`padding`](https://developer.mozilla.org/en-US/docs/Web/CSS/margin).

## 9. Footer Styling
- Create `<footer>` selector in the general CSS file.
- Set [`position`](https://developer.mozilla.org/en-US/docs/Web/CSS/position) to fixed.
- Set [`bottom`](https://developer.mozilla.org/en-US/docs/Web/CSS/bottom), [`left`](https://developer.mozilla.org/en-US/docs/Web/CSS/left), and [`right`](https://developer.mozilla.org/en-US/docs/Web/CSS/right) to 0.
- Set `background-color` and text `color`.
- Set [`height`](https://developer.mozilla.org/en-US/docs/Web/CSS/height) to an absolute value (e.g., in pixels).
  - *Why it's overlapping with `<body>` content?*
- Set [`text-align`](https://developer.mozilla.org/en-US/docs/Web/CSS/text-align) to center
  - *What's the problem?*  
- Optional: Add a [`background-image`](https://developer.mozilla.org/en-US/docs/Web/CSS/background-image) to the footer.

## 10. Navigation Bar (Optional, Time-Based) TODO:
- Similar to the footer, set position fixed.
- Remove style type.
- Set height, centering, and alignment.
- Optional: Set margin, font weight, color.

## 11. Adding Price/Contact Table
### 11.1 Contact-Prices CSS File
- Create a new CSS file *(`/Styles` folder)* for contact-prices HTML file.
- Create a new `<div>` around the `<table>` in contact-prices HTML file and assign a [`class="price-table"`](https://developer.mozilla.org/en-US/docs/Web/CSS/Class_selectors)selector to that `<div>`.

### 11.2 Table Styling
- Create a [descendant *(combinator)* selector](https://developer.mozilla.org/en-US/docs/Web/CSS/Descendant_combinator)  for the `<table>` under `price-table` class.
- Set [`width`](https://developer.mozilla.org/en-US/docs/Web/CSS/width), [`border-collapse`](https://developer.mozilla.org/en-US/docs/Web/CSS/border-collapse), and [`margin`](https://developer.mozilla.org/en-US/docs/Web/CSS/margin) for that descendant selector.

### 11.3 Table Headers and Cells Styling
-  Create a [descendant *(combinator)* selectors](https://developer.mozilla.org/en-US/docs/Web/CSS/Descendant_combinator)   for table headers (`<th>`) and also for data cells (`<td>`) under the `price-table` class.
- Set solid [`border`](https://developer.mozilla.org/en-US/docs/Web/CSS/border).
- Optional: Set [`text-align`](https://developer.mozilla.org/en-US/docs/Web/CSS/text-align), [`vertical-align`](https://developer.mozilla.org/en-US/docs/Web/CSS/vertical-align), and [`padding`](https://developer.mozilla.org/en-US/docs/Web/CSS/padding).

### 11.4 Optional Styles
- Differentiate styles for header cells and data cells (e.g., [`background-color`](https://developer.mozilla.org/en-US/docs/Web/CSS/background-color)).
