# Website for the Center for Advanced Urban Systems (CAUS)

Welcome! This is the official GitHub repository for the CAUS website. This file explains how to manage and update the website in a simple, non-technical way.

**Live Website Link:** [https://kaist-caus.github.io](https://kaist-caus.github.io)

---

## How to Update Website Content

You don't need to be a programmer to make changes! All updates can be done directly from the GitHub website. The entire website is contained in a single file: `index.html`.

### The Easiest Way to Edit: Step-by-Step

1.  **Find the file:** In this repository, click on the `index.html` file.
2.  **Open the editor:** On the top-right of the file view, click the small **pencil icon** (✎). This will open a simple web-based text editor.
3.  **Find the text you want to change:** The code might look intimidating, but you can easily find any text. Press `Ctrl + F` (on Windows) or `Cmd + F` (on Mac) to open a search box. Type a few words of the sentence you want to edit.
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
3.  To add a **new person**, carefully copy an entire "Profile Card" block of code and paste it right below another card. Then, change the details. A block looks like this:

    ```html
    <!-- Profile Card -->
    <div class="bg-gray-50 rounded-lg p-6 text-center shadow-sm">
        <img src="img/new_profile_photo.jpg" class="w-24 h-24 mx-auto rounded-full mb-4 object-cover" alt="Photo of [New Person's Name]">
        <h4 class="font-bold text-lg">[New Person's Name]</h4>
        <p class="text-sm text-gray-600 mt-1 h-16" data-lang-key="person_new_person_title">[New Person's Title]</p>
        <a href="[Link to their website]" target="_blank" class="text-blue-600 hover:underline text-sm mt-2 inline-block">
            <span data-lang-key="person_website">Website</span>
        </a>
    </div>
    ```

    * **Important:** Before you can use a new photo, you must first upload it to the `img` folder in this repository.
    * Change the image URL in `src="..."` to the correct path (e.g., `img/new_profile_photo.jpg`).
    * Change the name, title, and website link.
    * **For the title**, you will need to add a new entry in the `translations` object at the bottom of the file for both English and Korean.

### How to Update the English and Korean Text

Our website supports two languages. All the text is stored at the very bottom of the `index.html` file, inside the `<script>` section.

1.  Open the editor and scroll all the way to the bottom.
2.  You will find a `translations` object. It has an `en: { ... }` block for English and a `ko: { ... }` block for Korean.
3.  Find the key for the text you want to change (e.g., `about_title: "About CAUS"`) and edit the text within the quotes. Make sure to update it in both the `en` and `ko` sections!

---

## License Information

* **Code:** The website's source code (the `index.html` file) is licensed under the **MIT License**. This means anyone can reuse the code for free.
* **Content:** All text and images on the website are licensed under the **Creative Commons Attribution 4.0 (CC BY 4.0)**. This allows others to share and adapt our work, as long as they give credit to CAUS.


---
---

# 도시 인공지능 연구소 (CAUS) 웹사이트

환영합니다! 이 곳은 CAUS 웹사이트의 공식 GitHub 저장소입니다. 이 파일은 비전문가도 쉽게 웹사이트를 관리하고 업데이트할 수 있도록 돕기 위해 작성되었습니다.

**웹사이트 주소:** [https://kaist-caus.github.io](https://kaist-caus.github.io)

---

## 웹사이트 콘텐츠 업데이트 방법

프로그래머가 아니어도 괜찮습니다! 모든 업데이트는 GitHub 웹사이트에서 직접 할 수 있습니다. 전체 웹사이트는 `index.html`이라는 단일 파일에 포함되어 있습니다.

### 가장 쉬운 수정 방법: 단계별 안내

1.  **파일 찾기:** 저장소에서 `index.html` 파일을 클릭합니다.
2.  **편집기 열기:** 파일 보기의 오른쪽 상단에 있는 작은 **연필 아이콘** (✎)을 클릭합니다. 간단한 웹 기반 텍스트 편집기가 열립니다.
3.  **수정할 텍스트 찾기:** 코드가 복잡해 보일 수 있지만, `Ctrl + F` (Windows) 또는 `Cmd + F` (Mac)를 눌러 검색창을 열면 원하는 텍스트를 쉽게 찾을 수 있습니다. 수정하고 싶은 문장의 일부를 입력해 보세요.
4.  **내용 수정하기:** 텍스트를 조심스럽게 수정합니다. `<p>`, `>`, `"`와 같은 주변의 특수 문자가 실수로 삭제되지 않도록 주의하세요. 따옴표 안의 단어만 수정하면 됩니다.
5.  **변경사항 저장하기:** 페이지 하단으로 스크롤하면 **"Commit changes"** 섹션이 있습니다.
    * 첫 번째 입력란에 변경 사항에 대한 간단한 설명을 작성합니다 (예: "소개 문구 업데이트").
    * 녹색 **"Commit changes"** 버튼을 클릭합니다.

이것으로 끝입니다! 변경사항은 1~2분 내에 실제 웹사이트에 반영됩니다.

---

### 팀 구성원 정보 업데이트 및 추가 방법

과정은 매우 유사합니다.

1.  편집기에서 `index.html` 파일을 엽니다 (위의 1, 2단계).
2.  수정하고 싶은 사람의 이름을 검색합니다 (`Ctrl+F` / `Cmd+F`).
3.  **새로운 구성원 추가:** 기존 구성원의 "Profile Card" 코드 블록 전체를 조심스럽게 복사하여 다른 카드 바로 아래에 붙여넣습니다. 그 다음, 세부 정보를 수정합니다. 코드 블록은 다음과 같은 형태입니다.

    ```html
    <!-- Profile Card -->
    <div class="bg-gray-50 rounded-lg p-6 text-center shadow-sm">
        <img src="img/new_profile_photo.jpg" class="w-24 h-24 mx-auto rounded-full mb-4 object-cover" alt="Photo of [새 구성원 이름]">
        <h4 class="font-bold text-lg">[새 구성원 이름]</h4>
        <p class="text-sm text-gray-600 mt-1 h-16" data-lang-key="person_new_person_title">[새 구성원 직책]</p>
        <a href="[웹사이트 링크]" target="_blank" class="text-blue-600 hover:underline text-sm mt-2 inline-block">
            <span data-lang-key="person_website">Website</span>
        </a>
    </div>
    ```
    * **중요:** 새 프로필 사진을 사용하려면, 먼저 이 저장소의 `img` 폴더에 사진 파일을 업로드해야 합니다.
    * `src="..."` 안에 있는 이미지 주소를 올바른 경로로 변경합니다 (예: `img/new_profile_photo.jpg`).
    * 이름, 직책, 웹사이트 링크를 수정합니다.
    * **직책의 경우**, 파일 하단의 `translations` 객체에 영문과 국문 직책을 모두 추가해야 합니다.

### 영문/국문 텍스트 업데이트 방법

우리 웹사이트는 두 가지 언어를 지원합니다. 모든 텍스트는 `index.html` 파일의 가장 아래쪽 `<script>` 섹션 안에 저장되어 있습니다.

1.  편집기를 열고 페이지 맨 아래로 스크롤합니다.
2.  `translations` 객체를 찾을 수 있습니다. 여기에는 영문 텍스트를 위한 `en: { ... }` 블록과 국문 텍스트를 위한 `ko: { ... }` 블록이 있습니다.
3.  수정하려는 텍스트의 키(key)를 찾아서 (예: `about_title: "CAUS 소개"`) 따옴표 안의 내용을 수정합니다. 반드시 `en`과 `ko` 섹션 양쪽 모두를 업데이트해야 합니다!

---

## 라이선스 정보

* **코드:** 웹사이트의 소스 코드(`index.html` 파일)는 **MIT 라이선스**를 따릅니다. 누구나 자유롭게 코드를 재사용할 수 있습니다.
* **콘텐츠:** 웹사이트의 모든 텍스트와 이미지는 **Creative Commons Attribution 4.0 (CC BY 4.0)** 라이선스를 따릅니다. CAUS를 출처로 명시한다면 누구나 자유롭게 콘텐츠를 공유하고 수정할 수 있습니다.
