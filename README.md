# Modern Shopify Careers Page Section

A fully responsive, drag-and-drop Careers/Jobs section for Shopify Online Store 2.0 themes. This section features a split-view layout (Master-Detail pattern), dynamic category filtering, and an inline application form that works without page reloads.

## 🚀 Features

* **Split-View Layout:** Lists jobs on the left; shows full details (description, requirements, benefits) on the right without navigating away.
* **Dynamic Filtering:** Filter jobs by category (e.g., Corporate vs. Warehouse) instantly using JavaScript.
* **Inline Application Form:** The contact form appears directly below the job description when a user clicks "Apply."
* **Fail-Safe Logic:** Uses a state-based approach to ensure the correct Job Title is always sent with the application.
* **Mobile Responsive:** transforms into a stacked layout on mobile devices with smooth scroll interactions.
* **Fully Customizable:** All text, headings, and job data are managed via the Shopify Theme Editor (Schema settings).

## 🛠️ Technical Details

* **Language:** Shopify Liquid, HTML5, CSS3, Vanilla JavaScript (ES6).
* **Dependencies:** None (No jQuery required).
* **Form Handling:** Uses the native Shopify `{% form 'contact' %}`.
    * *Note:* Due to Shopify's native form limitations for non-Plus merchants, the "Resume" field accepts a URL (Google Drive/Dropbox link) rather than a file upload to ensure reliable delivery.

## 📦 Installation

1.  **Copy the Code:** Copy the contents of `sections/careers.liquid` from this repository.
2.  **Open Shopify Admin:** Go to **Online Store > Themes > Edit Code**.
3.  **Create Section:** Under the **Sections** folder, create a new file named `careers.liquid`.
4.  **Paste & Save:** Paste the code and hit save.
5.  **Add to Page:**
    * Go to the **Theme Customizer**.
    * Navigate to the page where you want the jobs listed.
    * Click **Add Section** and select **Careers**.

## ⚙️ Configuration

Inside the Shopify Theme Customizer, you can configure:

* **Headings:** Main title, subtitle, and department group titles.
* **Job Blocks:** Add individual job blocks. For each job, you can define:
    * Job Title
    * Category (Corporate/Warehouse)
    * Tags (Location, Type, On-site/Remote)
    * Rich text for About, Qualifications, Responsibilities, and Benefits.

## 📝 Usage

When a user applies:
1.  They select a job.
2.  They click "Apply Now" to reveal the inline form.
3.  They fill out their details and paste a link to their CV.
4.  Upon submission, the store owner receives an email notification via Shopify with the **Job Title** and applicant details included.

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
