---
layout: base
title: Student Home 
description: Home Page
hide: true
---

# Hi
Why hello there, my name is Aadit Mathur, and I am a high school student passionate about computer science.

Here is the link to my [Github](https://github.com/aaguy-hue).


# Bye
I greatly appreciate the fact that you spent time reading this webpage.

<button id="add-aadit">Add a picture of me!!!</button>
<div class="aadit-images">
</div>

<script>
    const btn = document.getElementById("add-aadit")
    btn.addEventListener("click", function() {
        const newImg = document.createElement("img");
        newImg.src = "/aadit_2025/images/aadit.jpg";
        newImg.alt = "Aadit";
        document.querySelector(".aadit-images").appendChild(newImg);
    });
</script>