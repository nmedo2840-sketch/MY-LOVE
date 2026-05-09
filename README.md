    document.getElementById("seconds").innerText = seconds;
}

setInterval(updateCounter,1000);
updateCounter();

/* 💖 قلوب طايرة */
function createHeart(){

    const heart = document.createElement("div");

    heart.classList.add("heart");

    heart.innerHTML = "❤";

    heart.style.left = Math.random() * 100 + "vw";

    heart.style.fontSize = (Math.random()*25 + 15) + "px";

    heart.style.animationDuration = (Math.random()*5 + 5) + "s";

    document.body.appendChild(heart);

    setTimeout(()=>{
        heart.remove();
    },10000);
}

setInterval(createHeart,300);

/* ✨ نجوم */
const stars = document.getElementById("stars");

for(let i=0;i<120;i++){

    const star = document.createElement("span");

    star.style.top = Math.random()*100 + "%";
    star.style.left = Math.random()*100 + "%";

    star.style.animationDelay = Math.random()*3 + "s";

    stars.appendChild(star);
}

</script>

</body>
</html>
