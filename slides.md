---
marp: true
theme: uncover # gaia
inlineSVG: true
description: A talk by Samir Rashid https://godsped.com
# class: 
#   - invert # dark mode
math: mathjax
# backgroundImage: "linear-gradient(to bottom, #67b8e3, #0288d1)"
paginate: true
transition: fade 

---
<style>
/* Font */
/* Body */
@font-face  {
    font-family: "lato";
    src: url("./font/Lato-Regular.ttf");
}
/* Title */
@font-face  {
    font-family: "raleway";
    src: url("./font/Raleway-SemiBold.ttf");
}
/* Code */
@font-face  {
    font-family: "hack";
    src: url("./font/Hack-Regular.ttf");
}

/* Global style */
section {
  background: #DFDFDA;
  font-family: 'lato', serif !important;
}

h1 {
    background: #C2C2BD;
    padding: 2%;
    color: #382D29;
    border-radius: 10px;
    font-family: 'raleway', serif !important;
}

h1, h2, h3, h4 {
    color: black;
    font-family: 'raleway', serif !important;
}

/* PNG image transparent background workaround (issue#119) */
img {
    background-color: transparent!important;
    border-radius:4%;
}

/* Code block */
pre {
  background: #f6f7f6;
  font-family: 'hack', serif !important;
   /* font-size: 2em; */
}

code {
  font-family: 'hack', serif !important;
}

/* Hyperlinks */
a {
    color: #2b7982;
}

/* Quote */
blockquote {
  color: black;
}

/* Two columns */
/* https://github.com/orgs/marp-team/discussions/62#discussioncomment-257185 */
div.twocols {
  /* margin-top: 35px; */
  column-count: 2;
}
div.twocols p:first-child,
div.twocols h1:first-child,
div.twocols h2:first-child,
div.twocols ul:first-child,
div.twocols ul li:first-child,
div.twocols ul li p:first-child {
  margin-top: 0 !important;
}
div.twocols p.break {
  break-before: column;
  margin-top: 0;
}

/* Center images with "center" label */
img[alt~="center"] {
  display: block;
  margin: 0 auto;
}

/* Clear background with "transparent" label */
img[alt~="transparent"] {
  mix-blend-mode: multiply;
}

/* figure {
  mix-blend-mode: multiply;
  background: #DFDFDA;
} */

/* Highlighting line in code block */
/* https://github.com/marp-team/marp-vscode/issues/146 */
.highlighted-line {
  background-color: #ff0;
  display: block;
  margin: 0 -16px;
  padding: 0 16px;
}

.reveal-items-list li {
  list-style-type: none;
}
.reveal-items-list ul {
  padding: 0;
  list-style: none; 
}

pre ol {
  padding: 0;
  margin: 0;
  list-style: none; 
}

pre li {
  padding: 0;
  margin: 0;
  list-style: none; 

}
</style>


<!-- 
cost of malware to UCSD
because devices are insecure and on the internet
- like insulin pumps
this is in Rust
- white house
- google
this is smart dust which can collect data, patient location using mesh networking without internet

round coin cell has x years of battery life
cost of this is x
open source and free

wearables allow for more data. and better patient outcomes.
thread can help patients even in remote areas

patient tracking low power amputees

 -->



<!-- _header: "" -->
<!-- _paginate: hide -->

# Secure Dust: reliable healthcare devices

## Low Cost. Low Power. Secure.

## **Samir Rashid**
<!-- ### Open Source Firmware Conference, September 3, 2024 -->

<br /> <br /> <br /> <br /> <br />

---

<style scoped>
  .image-container {
    display: flex;
    justify-content: space-between;
}

.image-container img {
    flex: 1;
    max-width: 33%;
    height: auto;
        object-fit: contain;

    margin: 0 10px; /* Adjust the margin as needed */
}
</style>

<div class="image-container">
    <img data-marpit-fragment src="./pacemaker.png" alt="transparent">
    <img data-marpit-fragment src="./insulin.png" alt="transparent">
</div>

---

![](./vuln.png)

---

![](./hack.png)


---

![](./money.png)
---

![](./rust.png)

---

# Security is **critical** and **urgent**.

---

> ## Chronic diseases account for 73% of deaths worldwide

<br>

> ## An estimated 36% of all allocated health care expenditure is directed at supporting individuals with chronic diseases

- [NIH](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC9288104/)

---

# Long term illnesses require long term monitoring

---

# Long term illnesses require **secure** long term monitoring

---

# Secure Dust: low-cost, low-power, secure wearables
![center](./15mm.png)

---

# Key Features:
1) **Real-time Monitoring**
   - Seamlessly connects to smartphones and health apps.
   - Allows for easy data sharing with healthcare providers.
   - Customizable alerts.
2) **Long Battery Life**
   - Energy-efficient design ensures extended usage between charges.
3) **Low Cost**
    - Off the shelf parts and optimized design.
4) **Secure Software**
    - Foundations for complying with future FDA regulations.

---



![center](./schematic.png)

---

![center](./layout.png)

---

![center](./pcb.png)

---

![center](./15mm.png)

---

# Tock OS
* embedded operating system
* used to secure millions of consumer devices

---

![center](./tock.png)

---

![](./thread.png)

---

# Summary

---

![center](./arrow.png)

---

# Game changer for **Elder Care** and **Chronic Conditions**

---

# Summary

* ## low cost ($5)
* ## low power (3µA)
  * ## up to 10 years of battery life
* ## operates without internet access
* ## open source foundation for secure medical devices

---

# Thanks! Questions?