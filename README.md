# Website for the Center for Advanced Urban Systems (CAUS)

Welcome! This is the official GitHub repository for the CAUS website. This file explains how to manage and update the website in a simple, non-technical way.

**Live Website Link:** [https://kaist-caus.github.io](https://kaist-caus.github.io)

---

## How to Update Website Content

You don't need to be a programmer to make changes! All updates can be done directly from the GitHub website. The entire website is contained in a single file: `index.html`.

### The Easiest Way to Edit: Step-by-Step

Let's say you want to change the description of a research area.

1.  **Find the file:** In this repository, click on the `index.html` file.
2.  **Open the editor:** On the top-right of the file view, click the small **pencil icon** (✎). This will open a simple web-based text editor.
3.  **Find the text you want to change:** The code might look intimidating, but you can easily find any text. Press `Ctrl + F` (on Windows) or `Cmd + F` (on Mac) to open a search box. Type a few words of the sentence you want to edit.
    * *Example:* To change the "About CAUS" text, you could search for "redefine urban living".
4.  **Make your changes:** Carefully edit the text. Be sure not to accidentally delete any of the surrounding characters like `<p>` or `>` or `"`. Just change the words inside.
5.  **Save your changes:** Scroll to the bottom of the page. You'll see a section called **"Commit changes"**.
    * In the first text box, briefly describe your change (e.g., "Updated About Us description").
    * Click the green **"Commit changes"** button.

That's it! Your changes will be live on the website within a minute or two.

---

### How to Update a Team Member or Add a New One

The process is very similar.

1.  Open the `index.html` file in the editor (steps 1 & 2 above).
2.  Search (`Ctrl+F` / `Cmd+F`) for the name of the person you want to edit.
3.  Change their name or title.
4.  To add a **new person**, carefully copy the entire block of code for an existing person and paste it right below. Then, change the details. A block looks like this:

    ```html
    <!-- Start of a person's block -->
    <div class="text-center">
        <img src="[https://placehold.co/400x400/a0aec0/ffffff?text=Prof.+F](https://placehold.co/400x400/a0aec0/ffffff?text=Prof.+F)" class="w-32 h-32 mx-auto rounded-full mb-4 shadow-md" alt="Researcher Photo">
        <h4 class="font-bold text-lg">Professor F</h4>
        <p class="text-sm text-gray-600" data-lang-key="people_role_6">New Role</p>
    </div>
    <!-- End of a person's block -->
    ```

    * Change the image URL in `src="..."` to a link for the new person's photo.
    * Change the name and title.

### How to Update the English and Korean Text

Our website supports two languages. All the text is stored at the very bottom of the `index.html` file, inside the `<script>` section.

1.  Open the editor and scroll all the way to the bottom.
2.  You will find a `translations` object. It has an `en: { ... }` block for English and a `ko: { ... }` block for Korean.
3.  Find the key for the text you want to change (e.g., `about_title: "About CAUS"`) and edit the text within the quotes. Make sure to update it in both the `en` and `ko` sections!

---

## License Information

* **Code:** The website's source code (the `index.html` file) is licensed under the **MIT License**. This means anyone can reuse the code for free.
* **Content:** All text and images on the website are licensed under the **Creative Commons Attribution 4.0 (CC BY 4.0)**. This allows others to share and adapt our work, as long as they give credit to CAUS.
