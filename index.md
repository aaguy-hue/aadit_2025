---
layout: base
title: Student Home 
description: Home Page
hide: true
---

<style>
    .aadit-images {
        display: grid;
        grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
        gap: 20px;
        margin-top: 20px;
    }
    .aadit-image {
        width: 100%;
        height: auto;
        border-radius: 8px;
        box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        transition: transform 0.3s ease;
    }
    .aadit-image:hover {
        transform: scale(1.05);
    }
    #add-aadit {
        padding: 10px 20px;
        font-size: 16px;
        cursor: pointer;
        border-radius: 5px;
        background-color: #4a5568;
        border: none;
        color: white;
        outline: none;
        transition: transform 0.1s ease-in-out;
    }
    #add-aadit:disabled {
        cursor: not-allowed;
        background-color: #a0aec0;
        transform: none;
        transition: none;
    }
    #add-aadit:active:not(:disabled) {
        transform: scale(1.1);
    }
    @keyframes clickEffect {
        0% { transform: scale(1); }
        50% { transform: scale(1.1); }
        100% { transform: scale(1); }
    }
    body {
        font-family: Arial, sans-serif;
        background-color: #1a202c;
        color: #fff;
        margin: 0;
        padding: 20px;
        min-height: 100vh;
        box-sizing: border-box;
    }
    .grid-container {
        display: grid;
        grid-template-columns: repeat(2, 1fr);
        gap: 20px;
        max-width: 1000px;
        margin: 0 auto;
    }
    .project-card {
        background-color: #2d3748;
        border-radius: 8px;
        padding: 20px;
        box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        transition: box-shadow 0.3s ease;
    }
    .project-card:hover {
        box-shadow: 0 10px 15px rgba(0, 0, 0, 0.2);
    }
    .project-title {
        font-size: 1.5em;
        margin-top: 0;
        margin-bottom: 10px;
    }
    .project-description {
        margin-bottom: 15px;
        color: #cbd5e0;
    }
    .project-link {
        color: #63b3ed;
        text-decoration: none;
        display: inline-flex;
        align-items: center;
    }
    .project-link:hover {
        text-decoration: underline;
    }
    .project-stats {
        float: right;
        color: #a0aec0;
    }
    .github-icon {
        width: 20px;
        height: 20px;
        margin-right: 5px;
    }

    .sprint-button {
        display: inline-flex;
        align-items: center;
        padding: 0.75rem 1.5rem;
        background: linear-gradient(135deg, #c92228, #5f22c9);
        color: white;
        text-decoration: none;
        border-radius: 8px;
        font-weight: 600;
        border: none;
        transition: all 0.3s ease;
        box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1);
    }

    .sprint-button:hover {
        transform: translateY(-2px);
        box-shadow: 0 6px 8px -1px rgba(0, 0, 0, 0.2);
    }

    .sprint-button:active {
        transform: translateY(0);
    }
</style>

# Hi
Why hello there, my name is Aadit Mathur, and I am a high school student passionate about computer science.

Here is the link to my [Github](https://github.com/aaguy-hue).

<br />

## My blogs 🗣️
<a href="{{site.baseurl}}/csa/sprint1/"><button class="sprint-button">Sprint 1</button></a>
<br />
<a href="{{site.baseurl}}/csa/notes/home/"><button class="sprint-button">Sprint 2 ― Notes Homepage</button></a>
<br />
<a href="{{site.baseurl}}/csa/mcq/2014"><button class="sprint-button">2014 MCQ Blog</button></a>
<br />
<a href="{{site.baseurl}}/blogs/student-panel"><button class="sprint-button">GICS Student Panel Blog</button></a>
<br />
<a href="{{site.baseurl}}/blogs/pbl-reflection"><button class="sprint-button">PBL Reflection Blog</button></a>
<br />
<a href="{{site.baseurl}}/blogs/docse/trimester-2-final"><button class="sprint-button">Trimester 2 - Last PBL Reflection</button></a>
<br />
<a href="{{site.baseurl}}/blogs/finalreview"><button class="sprint-button">Final Review Blog</button></a>
<br />

## ✨ Some Projects ✨
<div class="grid-container" id="projectGrid"></div>

<br />
<br />

# Bye
I greatly appreciate the fact that you spent time reading this webpage.


<button id="add-aadit">Add a picture of me!!!</button>
<div class="aadit-images">
</div>

<script src="https://utteranc.es/client.js"
        repo="aaguy-hue/aadit_2025"
        issue-term="pathname"
        label="blog_comment"
        theme="github-light"
        crossorigin="anonymous"
        async>
</script>

<script>
    const projects = [
        {
            title: "ImgGameLib",
            description: "A python game engine to create games based on images.",
            url: "https://github.com/aaguy-hue/ImgGameLib",
            stats: { stars: 0, forks: 0 }
        },
        {
            title: "CyberToolsBot",
            description: "A discord bot for cybersecurity tools.",
            url: "https://github.com/aaguy-hue/CyberToolsBot",
            stats: { stars: 0, forks: 0 }
        },
        {
            title: "8-Bit",
            description: "A discord bot for playing various games, was once in 50+ servers before being archived.",
            url: "https://github.com/aaguy-hue/8-Bit",
            stats: { stars: 1, forks: 0 }
        },
        {
            title: "SignUpBetter",
            description: "A website to create forms to sign up for things.",
            url: "https://github.com/aaguy-hue/SignUpBetter",
            stats: { stars: 1, forks: 0 }
        }
    ];

    function createProjectCard(project) {
        return `
            <div class="project-card">
                <h3 class="project-title">${project.title}</h3>
                <p class="project-description">${project.description}</p>
                <a href="${project.url}" class="project-link" target="_blank" rel="noopener noreferrer">
                    <svg class="github-icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                        <path d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22"></path>
                    </svg>
                    View on GitHub
                </a>
                <span class="project-stats">⭐ ${project.stats.stars} 🍴 ${project.stats.forks}</span>
            </div>
        `;
    }

    function renderProjects() {
        const projectGrid = document.getElementById('projectGrid');
        projectGrid.innerHTML = projects.map(createProjectCard).join('');
    }

    renderProjects();
</script>

<script>
const btn = document.getElementById("add-aadit");
const imageContainer = document.querySelector(".aadit-images");
let imageCount = 0;
const maxImages = 10;

btn.addEventListener("click", function() {
    if (imageCount < maxImages) {
        const newImg = document.createElement("img");
        newImg.src = "{{ '/images/aadit.jpg' | relative_url }}";
        newImg.alt = "Picture of Aadit";
        newImg.classList.add("aadit-image");
        imageContainer.appendChild(newImg);
        imageCount++;

        if (imageCount === maxImages) {
            btn.disabled = true;
            btn.textContent = "Please chill";
        }
    }
});

</script>