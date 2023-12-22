
### Hi, I'm Jaime Suarez ...
### <img src="https://media1.giphy.com/media/l8gL23OcJmthB2Yv2E/200w.webp?cid=ecf05e47q1kfyj1qcv9owagiyoya6udsyjgb67s6kblxdext&ep=v1_gifs_search&rid=200w.webp&ct=g" width="50"> A little more about me...

```javascript

let currentIndex = 0;
const images = [
  "https://drive.google.com/uc?id=1ETCw0myX3LQDe4sVoYp7sigKcQ49xPmH",
  "https://drive.google.com/uc?id=1Ze2aYHEZNUCtblz0OCL5vmhb_ucol978",
  "https://drive.google.com/uc?id=1cYYVYw1JEg813lCJyEyVHjEp2hxHrKti"
];

function showImage(index) {
  const imageElement = document.getElementById('slideshow-image');
  imageElement.src = images[index];
}

function nextImage() {
  currentIndex = (currentIndex + 1) % images.length;
  showImage(currentIndex);
}

// Cambiar a la siguiente imagen cada 3 segundos (ajusta el tiempo según sea necesario)
setInterval(nextImage, 3000);

// Mostrar la primera imagen al cargar la página
document.write('<div id="slideshow-container"><img id="slideshow-image" src="https://drive.google.com/uc?id=1ETCw0myX3LQDe4sVoYp7sigKcQ49xPmH" width="300"></div>');
