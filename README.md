# BrightPath Digital Studio — Week 4 Complete Business Website

A four-page, responsive professional services website created for the Week 4 web development assignment using HTML5, CSS3 and vanilla JavaScript.

> **Project type:** Educational/demo project. BrightPath Digital Studio is a fictional business. The contact form performs browser-side validation only and does not deliver messages.

## 1. Project overview

The website demonstrates how a small business can present its identity, explain its services and invite potential customers to make contact. The design uses a consistent navigation system, clear content hierarchy, responsive layouts and accessible form controls.

## 2. Pages

- `index.html` — home page, introduction, service highlights and call to action.
- `about.html` — business story, approach and values.
- `services.html` — detailed service descriptions.
- `contact.html` — contact information and validated enquiry form.

## 3. Folder structure

```text
week4-business-website/
├── index.html
├── about.html
├── services.html
├── contact.html
├── css/
│   └── style.css
├── js/
│   └── main.js
├── images/
│   ├── hero-illustration.svg
│   └── team-illustration.svg
└── README.md
```

## 4. Setup instructions

1. Download and extract the ZIP file.
2. Open the extracted `week4-business-website` folder in VS Code.
3. Open `index.html` in a browser, or use the VS Code Live Server extension.
4. Use the navigation links to visit all four pages.
5. Test the contact form with both invalid and valid details.

No package installation, framework or build command is required. Google Fonts are loaded from the internet; system fallback fonts are provided.

## 5. Design decisions

- **Business option:** Professional Services Website.
- **Brand:** BrightPath Digital Studio (fictional).
- **Visual style:** clean, modern and professional, with a purple accent palette and generous spacing.
- **Layout:** shared header and footer, reusable cards, consistent buttons and a responsive grid.
- **Mobile-first behaviour:** navigation collapses into a menu on smaller screens; grids become single-column on narrow screens.

## 6. Functionality

- Navigation links connect all four HTML pages.
- Mobile navigation opens and closes with a button.
- Contact form validates name, email, service selection and message length.
- Field-level error messages are shown beside invalid inputs.
- Error messages clear as the user edits fields.
- Copyright year is inserted dynamically using JavaScript.
- Semantic landmarks, descriptive image alt text, visible keyboard focus, a skip link, form labels and live status feedback support accessibility.

## 7. Technical details

- **Architecture:** multi-page static website. Each HTML page loads the shared `css/style.css` and `js/main.js` files.
- **HTML:** semantic `header`, `nav`, `main`, `section`, `article` and `footer` elements.
- **CSS:** CSS custom properties, Grid, Flexbox, media queries and reduced-motion preference.
- **JavaScript:** DOM selection, reusable `setError()` and `validateForm()` functions, event listeners (`click`, `submit`, `input`, `change`), regular-expression email validation and conditional checks.
- **Data handling:** form values are read in the browser and are not sent to a server.
- **Images:** custom SVG illustrations are scalable vector assets and do not require large photographic files.

## 8. Testing evidence

| Test | Action | Expected result |
|---|---|---|
| Page navigation | Click Home, About, Services and Contact | Each page opens correctly |
| Mobile menu | Reduce browser width and click menu | Menu opens/closes and `aria-expanded` changes |
| Empty form | Submit with all fields empty | Field-specific error messages appear |
| Short name | Enter one character | Name validation error appears |
| Invalid email | Enter `abc` | Email validation error appears |
| Missing service | Leave service unselected | Service validation error appears |
| Short message | Enter fewer than 10 characters | Message validation error appears |
| Valid form | Complete all fields correctly | Success confirmation appears |
| Responsive layout | Check desktop, tablet and phone widths | Content reflows without horizontal scrolling |

## 9. Performance and compatibility

- SVG illustrations are lightweight, scalable vector files.
- No external JavaScript libraries or frameworks are required.
- CSS media queries adapt the layout to smaller screens.
- Use current versions of Chrome, Edge, Firefox and Safari for testing.
- Google Fonts require an internet connection; fallback fonts are defined.

## 10. Deployment using GitHub Pages

1. Create a GitHub repository, for example `week4-business-website`.
2. Upload the **contents** of this project folder to the repository root. The `index.html` file must be at the root.
3. Open the repository on GitHub and select **Settings**.
4. Open **Pages** from the left sidebar.
5. Under **Build and deployment**, choose **Deploy from a branch**.
6. Select branch `main` and folder `/ (root)`, then click **Save**.
7. Wait for GitHub Pages to publish the site. The published URL will appear in the Pages settings.

Alternative: drag the project folder into Netlify Drop at https://app.netlify.com/drop (sign in may be required).

## 11. Before submission

- Replace the fictional business name and contact details if your instructor expects an original business.
- Add your own screenshots of the Home, About, Services and Contact pages.
- Test every page and form case on your own device.
- Include your actual published GitHub Pages or Netlify URL in your submission.
- Do not describe the demo form as a real booking or email system; a backend or form service is needed to receive messages.
