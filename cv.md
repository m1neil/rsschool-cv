# Alekseyev Eric

## My contacts

- **Location:** Ukraine Kharkov
- **Phone:** +380-98-983-05-99
- **E-mail:** ericalex0207@gmail.com
- **GitHub:** [Eric Alekseyev](https://github.com/m1neil)

## About Me

**Education:** Software Engineering student at Kharkiv National Automobile and Highway University (KhNAHU), Ukraine Kharkov.

**Objective:** My objective is to build a successful career in the field of software engineering, with a focus on front-end development. I am passionate about creating user-friendly and visually appealing websites and applications. I strive to continuously learn and stay updated with the latest trends and technologies in the industry.

**Strengths:** I'm highly self-motivated and take initiative to learn and explore new concepts independently. I pay great attention to detail, ensuring that my work is precise and of high quality. I'm a collaborative team player and believe in effective communication and cooperation to achieve common goals.

**Self-study:** While I don't have work experience, I have been actively engaged in enhancing my skills in front-end development. I have been taking various online courses on platforms like Udemy and watching educational videos on YouTube. These resources have helped me gain practical knowledge and hands-on experience in HTML, CSS, JavaScript, and other relevant technologies. I have been working on personal projects to apply what I have learned and improve my proficiency.

## Skills

- HTML
- CSS (Preprocessor SCSS, BEM methodology).
- JavaScript (Fundamentals, Functional Programming, OOP, Asynchronous JavaScript+-, ES6+,DOM,JSON).
- Version control: Git (remote service GitHub).
- Module Bundlers: Gulp, Webpack.
- C++ (basic knowledge), Python(basic knowledge), SQLite3(basic knowledge), PHP(basic knowledge) MySQL(basic knowledge)
- Windows OS
- Figma, Avacode, Zeplin, Inspect, Adobe Photoshop, (for web development)
- Editors: VSCode.

## Code

`export default function tabs(selector, itemStorage = 'index') {
console.log(selector.length);
if (selector.length) {
const tabsContainer = document.querySelector(selector);
if (tabsContainer) {
const navMenuLink = tabsContainer.querySelectorAll('.tabs**link-tab'),
tabs = tabsContainer.querySelectorAll('.tabs**tab');

    		checkLocalStorageTabs();

    		navMenuLink.forEach((link, index) => {
    			link.addEventListener("click", function (e) {
    				e.preventDefault();
    				deleteClassActive();
    				console.log(index);
    				addClassActive(index);
    				localStorage.setItem(`${itemStorage}`, index);
    			});
    		});

    		function deleteClassActive() {
    			navMenuLink.forEach(item => item.classList.remove('active'));
    			tabs.forEach(tab => tab.classList.remove('active'));
    		}

    		function addClassActive(tabIndex = 0) {
    			navMenuLink[tabIndex].classList.add('active');
    			tabs[tabIndex].classList.add('active');
    		}

    		function checkLocalStorageTabs() {
    			if (localStorage.getItem(`${itemStorage}`)) {
    				addClassActive(localStorage.getItem(`${itemStorage}`))
    			} else {
    				addClassActive();
    			}
    		}
    	}
    }

}`
