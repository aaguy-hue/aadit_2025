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
        transition: background-color 0.3s ease;
    }
</style>

# Hi
Why hello there, my name is Aadit Mathur, and I am a high school student passionate about computer science.

Here is the link to my [Github](https://github.com/aaguy-hue).


# Bye
I greatly appreciate the fact that you spent time reading this webpage.

<button id="add-aadit">Add a picture of me!!!</button>
<div class="aadit-images">
</div>

<script>
const btn = document.getElementById("add-aadit");
const imageContainer = document.querySelector(".aadit-images");
let imageCount = 0;
const maxImages = 10;

btn.addEventListener("click", function() {
    if (imageCount < maxImages) {
        const newImg = document.createElement("img");
        newImg.src = "/aadit_2025/images/aadit.jpg";
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