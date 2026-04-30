#Cloudy BeansCafé Website

## Project overview

This website presents cloudy beans cafe wesbsite that will offer cakes,drinks and Free wifi.

The website contains three pages:

- `index.html` - home page and café introduction
- `pages/menu.html` - food and drink menu
- `pages/contact.html` - contact details and functional demo booking form

## Design

### Aims and objectives

The aim of the website is to provide customers with clear information about the café and encourage them to visit or make a booking The objectives are:

- present the café brand using warm colours and accessible contrast
- make the site easy to use on desktop, tablet, and mobile screens
- provide clear navigation between pages
- display a menu with prices
- allow customers to submit a booking/contact form
- include interactive features controlled by the user

### User stories

- As a customer, I want to view the café menu so that I can decide what to order before visiting.
- As a customer, I want to find contact details so that I can ask questions or book a table.
- As a mobile user, I want the website to resize properly so that I can use it on my phone.
- As a visually impaired user, I want images to have alternative text and colours to have enough contrast.
- As a user, I want control over pop-ups and audio so that nothing opens or plays without my permission.

### Wireframes

Wireframes were planned around a simple three-page structure:

1. Home page: header navigation, hero section, feature cards, weather widget, and audio control.
2. Menu page: title section, image, menu cards, and user-controlled offer modal.
3. Contact page: title section, image, booking form, and café information panel.

The wireframes were revised during development to use a card-based layout because it works well with CSS Grid and adapts cleanly to mobile screens.

## Development

### Technologies used

- HTML5 for page structure
- CSS3 for layout, colour, typography, and responsive design
- JavaScript for the modal, form response, and weather API
- Open-Meteo API for the dynamic weather feature
- Git and GitHub for version control and deployment

### Key features

- Three distinct pages
- Main navigation menu on every page
- Responsive layout using CSS Grid and media queries
- Functional demo contact form with JavaScript confirmation message
- User-controlled modal pop-up on the menu page
- Alternative text for all images
- External links open in a new tab using `target="_blank"`
- Clean project folder structure

### File structure

```text
cafe_assignment_done/
├── css/
│   └── style.css
├── images/
│   ├── cafe-chime.wav
│   ├── contact-cafe.svg
│   ├── hero-cafe.svg
│   └── menu-coffee.svg


### Reflection

During development, the main challenge was making sure that links to CSS, JavaScript, and images worked correctly across pages in different folders. This was solved by using relative paths carefully: the home page uses paths such as `css/style.css`, while pages inside the `pages` folder use paths such as `../css/style.css`.

A warm café colour palette was chosen to match the topic and create a clear visual identity. CSS Grid was used because it makes the layout easier to control and allows the site to switch from multi-column cards on desktop to single-column content on smaller screens.

## Testing

### Manual testing

| Test | Expected result | Result |
|---|---|---|
| Open `index.html` | Home page loads with colours and image | Pass |
| Click Home navigation | Home page opens | Pass |
| Click Menu navigation | Menu page opens | Pass |
| Click Contact navigation | Contact page opens | Pass |
| Open external Instagram/Reviews/Map links | Links open in a new tab | Pass |
| Resize browser to mobile width | Cards stack into one column | Pass |
| Click student offer button | Pop-up opens | Pass |
| Click close pop-up button | Pop-up closes | Pass |
| Press play on audio | Audio plays only when user starts it | Pass |
| Submit empty contact form | Browser shows required field validation | Pass |

### User story testing

| User story | How it was tested | Result |
|---|---|---|
| View the menu before visiting | Opened menu page and checked menu items and prices | Pass |
| Find contact details | Opened contact page and checked address, hours, and form | Pass |
| Use site on mobile | Resized browser and checked responsive layout | Pass |
| Accessibility support | Checked image alt text, labels, focus styles, and contrast | Pass |
| User controls for media/pop-ups | Confirmed modal and audio only start through user action | Pass |

### Bugs found and fixed

| Bug | Fix |
|---|---|
| CSS and images did not load when pages were in folders | Corrected relative paths using `../` on pages inside the `pages` directory |
| Form originally had no response after submission | Added JavaScript confirmation message |
| Modal needed user control | Added open and close buttons |


Suggested Lighthouse results section:

- Performance: Add score after testing
- Accessibility: Add score after testing
- SEO: Add score after testing

## Version control

Git should be used throughout development. Example meaningful commit messages:

- `Create basic cafe website structure`
- `Add responsive CSS layout`
- `Add menu and contact pages`
- `Fix image and stylesheet paths`

## Attribution

- Responsive navigation idea adapted from W3Schools: https://www.w3schools.com/howto/howto_js_topnav_responsive.asp
- CSS Grid and media query ideas adapted from W3Schools: https://www.w3schools.com/css/css_grid.asp and https://www.w3schools.com/css/css_rwd_mediaqueries.asp
- Modal interaction idea adapted from W3Schools: https://www.w3schools.com/howto/howto_css_modals.asp
- HTML form structure adapted from W3Schools: https://www.w3schools.com/html/html_forms.asp
- Dynamic weather data from Open-Meteo: https://open-meteo.com/

