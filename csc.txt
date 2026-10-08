console.log("Mohit Cyber Cafe Website Loaded!");


// Smooth scrolling

document.querySelectorAll('a[href^="#"]').forEach(function(link) {

    link.addEventListener("click", function(event) {

        const section = document.querySelector(
            this.getAttribute("href")
        );

        if (section) {

            event.preventDefault();

            section.scrollIntoView({
                behavior: "smooth"
            });

        }

    });

});